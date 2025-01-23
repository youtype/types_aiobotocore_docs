# Type definitions

> [Index](../README.md) > [IoT](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#iot)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AddThingsToThingGroupParamsUnionTypeDef

```python
# AddThingsToThingGroupParamsUnionTypeDef definition

AddThingsToThingGroupParamsUnionTypeDef = Union[
    AddThingsToThingGroupParamsTypeDef,  # (1)
    AddThingsToThingGroupParamsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AddThingsToThingGroupParamsTypeDef](./type_defs.md#addthingstothinggroupparamstypedef) 
2. See [:material-code-braces: AddThingsToThingGroupParamsOutputTypeDef](./type_defs.md#addthingstothinggroupparamsoutputtypedef) 

## AttributePayloadUnionTypeDef

```python
# AttributePayloadUnionTypeDef definition

AttributePayloadUnionTypeDef = Union[
    AttributePayloadTypeDef,  # (1)
    AttributePayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) 
2. See [:material-code-braces: AttributePayloadOutputTypeDef](./type_defs.md#attributepayloadoutputtypedef) 

## AuthInfoUnionTypeDef

```python
# AuthInfoUnionTypeDef definition

AuthInfoUnionTypeDef = Union[
    AuthInfoTypeDef,  # (1)
    AuthInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthInfoTypeDef](./type_defs.md#authinfotypedef) 
2. See [:material-code-braces: AuthInfoOutputTypeDef](./type_defs.md#authinfooutputtypedef) 

## MetricValueUnionTypeDef

```python
# MetricValueUnionTypeDef definition

MetricValueUnionTypeDef = Union[
    MetricValueTypeDef,  # (1)
    MetricValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) 
2. See [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 

## CodeSigningSignatureUnionTypeDef

```python
# CodeSigningSignatureUnionTypeDef definition

CodeSigningSignatureUnionTypeDef = Union[
    CodeSigningSignatureTypeDef,  # (1)
    CodeSigningSignatureOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CodeSigningSignatureTypeDef](./type_defs.md#codesigningsignaturetypedef) 
2. See [:material-code-braces: CodeSigningSignatureOutputTypeDef](./type_defs.md#codesigningsignatureoutputtypedef) 

## CommandParameterValueUnionTypeDef

```python
# CommandParameterValueUnionTypeDef definition

CommandParameterValueUnionTypeDef = Union[
    CommandParameterValueTypeDef,  # (1)
    CommandParameterValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CommandParameterValueTypeDef](./type_defs.md#commandparametervaluetypedef) 
2. See [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 

## IndexingFilterUnionTypeDef

```python
# IndexingFilterUnionTypeDef definition

IndexingFilterUnionTypeDef = Union[
    IndexingFilterTypeDef,  # (1)
    IndexingFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IndexingFilterTypeDef](./type_defs.md#indexingfiltertypedef) 
2. See [:material-code-braces: IndexingFilterOutputTypeDef](./type_defs.md#indexingfilteroutputtypedef) 

## KafkaActionUnionTypeDef

```python
# KafkaActionUnionTypeDef definition

KafkaActionUnionTypeDef = Union[
    KafkaActionTypeDef,  # (1)
    KafkaActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KafkaActionTypeDef](./type_defs.md#kafkaactiontypedef) 
2. See [:material-code-braces: KafkaActionOutputTypeDef](./type_defs.md#kafkaactionoutputtypedef) 

## Mqtt5ConfigurationUnionTypeDef

```python
# Mqtt5ConfigurationUnionTypeDef definition

Mqtt5ConfigurationUnionTypeDef = Union[
    Mqtt5ConfigurationTypeDef,  # (1)
    Mqtt5ConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: Mqtt5ConfigurationTypeDef](./type_defs.md#mqtt5configurationtypedef) 
2. See [:material-code-braces: Mqtt5ConfigurationOutputTypeDef](./type_defs.md#mqtt5configurationoutputtypedef) 

## MqttHeadersUnionTypeDef

```python
# MqttHeadersUnionTypeDef definition

MqttHeadersUnionTypeDef = Union[
    MqttHeadersTypeDef,  # (1)
    MqttHeadersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MqttHeadersTypeDef](./type_defs.md#mqttheaderstypedef) 
2. See [:material-code-braces: MqttHeadersOutputTypeDef](./type_defs.md#mqttheadersoutputtypedef) 

## TimestreamActionUnionTypeDef

```python
# TimestreamActionUnionTypeDef definition

TimestreamActionUnionTypeDef = Union[
    TimestreamActionTypeDef,  # (1)
    TimestreamActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TimestreamActionTypeDef](./type_defs.md#timestreamactiontypedef) 
2. See [:material-code-braces: TimestreamActionOutputTypeDef](./type_defs.md#timestreamactionoutputtypedef) 

## PutAssetPropertyValueEntryUnionTypeDef

```python
# PutAssetPropertyValueEntryUnionTypeDef definition

PutAssetPropertyValueEntryUnionTypeDef = Union[
    PutAssetPropertyValueEntryTypeDef,  # (1)
    PutAssetPropertyValueEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef) 
2. See [:material-code-braces: PutAssetPropertyValueEntryOutputTypeDef](./type_defs.md#putassetpropertyvalueentryoutputtypedef) 

## HttpActionUnionTypeDef

```python
# HttpActionUnionTypeDef definition

HttpActionUnionTypeDef = Union[
    HttpActionTypeDef,  # (1)
    HttpActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HttpActionTypeDef](./type_defs.md#httpactiontypedef) 
2. See [:material-code-braces: HttpActionOutputTypeDef](./type_defs.md#httpactionoutputtypedef) 

## BehaviorCriteriaUnionTypeDef

```python
# BehaviorCriteriaUnionTypeDef definition

BehaviorCriteriaUnionTypeDef = Union[
    BehaviorCriteriaTypeDef,  # (1)
    BehaviorCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BehaviorCriteriaTypeDef](./type_defs.md#behaviorcriteriatypedef) 
2. See [:material-code-braces: BehaviorCriteriaOutputTypeDef](./type_defs.md#behaviorcriteriaoutputtypedef) 

## CustomCodeSigningUnionTypeDef

```python
# CustomCodeSigningUnionTypeDef definition

CustomCodeSigningUnionTypeDef = Union[
    CustomCodeSigningTypeDef,  # (1)
    CustomCodeSigningOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomCodeSigningTypeDef](./type_defs.md#customcodesigningtypedef) 
2. See [:material-code-braces: CustomCodeSigningOutputTypeDef](./type_defs.md#customcodesigningoutputtypedef) 

## CommandParameterUnionTypeDef

```python
# CommandParameterUnionTypeDef definition

CommandParameterUnionTypeDef = Union[
    CommandParameterTypeDef,  # (1)
    CommandParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CommandParameterTypeDef](./type_defs.md#commandparametertypedef) 
2. See [:material-code-braces: CommandParameterOutputTypeDef](./type_defs.md#commandparameteroutputtypedef) 

## RepublishActionUnionTypeDef

```python
# RepublishActionUnionTypeDef definition

RepublishActionUnionTypeDef = Union[
    RepublishActionTypeDef,  # (1)
    RepublishActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RepublishActionTypeDef](./type_defs.md#republishactiontypedef) 
2. See [:material-code-braces: RepublishActionOutputTypeDef](./type_defs.md#republishactionoutputtypedef) 

## IotSiteWiseActionUnionTypeDef

```python
# IotSiteWiseActionUnionTypeDef definition

IotSiteWiseActionUnionTypeDef = Union[
    IotSiteWiseActionTypeDef,  # (1)
    IotSiteWiseActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IotSiteWiseActionTypeDef](./type_defs.md#iotsitewiseactiontypedef) 
2. See [:material-code-braces: IotSiteWiseActionOutputTypeDef](./type_defs.md#iotsitewiseactionoutputtypedef) 

## BehaviorUnionTypeDef

```python
# BehaviorUnionTypeDef definition

BehaviorUnionTypeDef = Union[
    BehaviorTypeDef,  # (1)
    BehaviorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) 
2. See [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 

## CodeSigningUnionTypeDef

```python
# CodeSigningUnionTypeDef definition

CodeSigningUnionTypeDef = Union[
    CodeSigningTypeDef,  # (1)
    CodeSigningOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CodeSigningTypeDef](./type_defs.md#codesigningtypedef) 
2. See [:material-code-braces: CodeSigningOutputTypeDef](./type_defs.md#codesigningoutputtypedef) 

## ActionUnionTypeDef

```python
# ActionUnionTypeDef definition

ActionUnionTypeDef = Union[
    ActionTypeDef,  # (1)
    ActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 

## OTAUpdateFileUnionTypeDef

```python
# OTAUpdateFileUnionTypeDef definition

OTAUpdateFileUnionTypeDef = Union[
    OTAUpdateFileTypeDef,  # (1)
    OTAUpdateFileOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OTAUpdateFileTypeDef](./type_defs.md#otaupdatefiletypedef) 
2. See [:material-code-braces: OTAUpdateFileOutputTypeDef](./type_defs.md#otaupdatefileoutputtypedef) 



## AbortCriteriaTypeDef

```python
# AbortCriteriaTypeDef definition

class AbortCriteriaTypeDef(TypedDict):
    failureType: JobExecutionFailureTypeType,  # (1)
    action: AbortActionType,  # (2)
    thresholdPercentage: float,
    minNumberOfExecutedThings: int,
```

1. See [:material-code-brackets: JobExecutionFailureTypeType](./literals.md#jobexecutionfailuretypetype) 
2. See [:material-code-brackets: AbortActionType](./literals.md#abortactiontype) 
## AcceptCertificateTransferRequestRequestTypeDef

```python
# AcceptCertificateTransferRequestRequestTypeDef definition

class AcceptCertificateTransferRequestRequestTypeDef(TypedDict):
    certificateId: str,
    setAsActive: NotRequired[bool],
```

## CloudwatchAlarmActionTypeDef

```python
# CloudwatchAlarmActionTypeDef definition

class CloudwatchAlarmActionTypeDef(TypedDict):
    roleArn: str,
    alarmName: str,
    stateReason: str,
    stateValue: str,
```

## CloudwatchLogsActionTypeDef

```python
# CloudwatchLogsActionTypeDef definition

class CloudwatchLogsActionTypeDef(TypedDict):
    roleArn: str,
    logGroupName: str,
    batchMode: NotRequired[bool],
```

## CloudwatchMetricActionTypeDef

```python
# CloudwatchMetricActionTypeDef definition

class CloudwatchMetricActionTypeDef(TypedDict):
    roleArn: str,
    metricNamespace: str,
    metricName: str,
    metricValue: str,
    metricUnit: str,
    metricTimestamp: NotRequired[str],
```

## DynamoDBActionTypeDef

```python
# DynamoDBActionTypeDef definition

class DynamoDBActionTypeDef(TypedDict):
    tableName: str,
    roleArn: str,
    hashKeyField: str,
    hashKeyValue: str,
    operation: NotRequired[str],
    hashKeyType: NotRequired[DynamoKeyTypeType],  # (1)
    rangeKeyField: NotRequired[str],
    rangeKeyValue: NotRequired[str],
    rangeKeyType: NotRequired[DynamoKeyTypeType],  # (1)
    payloadField: NotRequired[str],
```

1. See [:material-code-brackets: DynamoKeyTypeType](./literals.md#dynamokeytypetype) 
2. See [:material-code-brackets: DynamoKeyTypeType](./literals.md#dynamokeytypetype) 
## ElasticsearchActionTypeDef

```python
# ElasticsearchActionTypeDef definition

class ElasticsearchActionTypeDef(TypedDict):
    roleArn: str,
    endpoint: str,
    index: str,
    type: str,
    id: str,
```

## FirehoseActionTypeDef

```python
# FirehoseActionTypeDef definition

class FirehoseActionTypeDef(TypedDict):
    roleArn: str,
    deliveryStreamName: str,
    separator: NotRequired[str],
    batchMode: NotRequired[bool],
```

## IotAnalyticsActionTypeDef

```python
# IotAnalyticsActionTypeDef definition

class IotAnalyticsActionTypeDef(TypedDict):
    channelArn: NotRequired[str],
    channelName: NotRequired[str],
    batchMode: NotRequired[bool],
    roleArn: NotRequired[str],
```

## IotEventsActionTypeDef

```python
# IotEventsActionTypeDef definition

class IotEventsActionTypeDef(TypedDict):
    inputName: str,
    roleArn: str,
    messageId: NotRequired[str],
    batchMode: NotRequired[bool],
```

## KinesisActionTypeDef

```python
# KinesisActionTypeDef definition

class KinesisActionTypeDef(TypedDict):
    roleArn: str,
    streamName: str,
    partitionKey: NotRequired[str],
```

## LambdaActionTypeDef

```python
# LambdaActionTypeDef definition

class LambdaActionTypeDef(TypedDict):
    functionArn: str,
```

## OpenSearchActionTypeDef

```python
# OpenSearchActionTypeDef definition

class OpenSearchActionTypeDef(TypedDict):
    roleArn: str,
    endpoint: str,
    index: str,
    type: str,
    id: str,
```

## S3ActionTypeDef

```python
# S3ActionTypeDef definition

class S3ActionTypeDef(TypedDict):
    roleArn: str,
    bucketName: str,
    key: str,
    cannedAcl: NotRequired[CannedAccessControlListType],  # (1)
```

1. See [:material-code-brackets: CannedAccessControlListType](./literals.md#cannedaccesscontrollisttype) 
## SalesforceActionTypeDef

```python
# SalesforceActionTypeDef definition

class SalesforceActionTypeDef(TypedDict):
    token: str,
    url: str,
```

## SnsActionTypeDef

```python
# SnsActionTypeDef definition

class SnsActionTypeDef(TypedDict):
    targetArn: str,
    roleArn: str,
    messageFormat: NotRequired[MessageFormatType],  # (1)
```

1. See [:material-code-brackets: MessageFormatType](./literals.md#messageformattype) 
## SqsActionTypeDef

```python
# SqsActionTypeDef definition

class SqsActionTypeDef(TypedDict):
    roleArn: str,
    queueUrl: str,
    useBase64: NotRequired[bool],
```

## StepFunctionsActionTypeDef

```python
# StepFunctionsActionTypeDef definition

class StepFunctionsActionTypeDef(TypedDict):
    stateMachineName: str,
    roleArn: str,
    executionNamePrefix: NotRequired[str],
```

## MetricValueOutputTypeDef

```python
# MetricValueOutputTypeDef definition

class MetricValueOutputTypeDef(TypedDict):
    count: NotRequired[int],
    cidrs: NotRequired[List[str]],
    ports: NotRequired[List[int]],
    number: NotRequired[float],
    numbers: NotRequired[List[float]],
    strings: NotRequired[List[str]],
```

## ViolationEventAdditionalInfoTypeDef

```python
# ViolationEventAdditionalInfoTypeDef definition

class ViolationEventAdditionalInfoTypeDef(TypedDict):
    confidenceLevel: NotRequired[ConfidenceLevelType],  # (1)
```

1. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype) 
## AddThingToBillingGroupRequestRequestTypeDef

```python
# AddThingToBillingGroupRequestRequestTypeDef definition

class AddThingToBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: NotRequired[str],
    billingGroupArn: NotRequired[str],
    thingName: NotRequired[str],
    thingArn: NotRequired[str],
```

## AddThingToThingGroupRequestRequestTypeDef

```python
# AddThingToThingGroupRequestRequestTypeDef definition

class AddThingToThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: NotRequired[str],
    thingGroupArn: NotRequired[str],
    thingName: NotRequired[str],
    thingArn: NotRequired[str],
    overrideDynamicGroups: NotRequired[bool],
```

## AddThingsToThingGroupParamsOutputTypeDef

```python
# AddThingsToThingGroupParamsOutputTypeDef definition

class AddThingsToThingGroupParamsOutputTypeDef(TypedDict):
    thingGroupNames: List[str],
    overrideDynamicGroups: NotRequired[bool],
```

## AddThingsToThingGroupParamsTypeDef

```python
# AddThingsToThingGroupParamsTypeDef definition

class AddThingsToThingGroupParamsTypeDef(TypedDict):
    thingGroupNames: Sequence[str],
    overrideDynamicGroups: NotRequired[bool],
```

## AggregationTypeOutputTypeDef

```python
# AggregationTypeOutputTypeDef definition

class AggregationTypeOutputTypeDef(TypedDict):
    name: AggregationTypeNameType,  # (1)
    values: NotRequired[List[str]],
```

1. See [:material-code-brackets: AggregationTypeNameType](./literals.md#aggregationtypenametype) 
## AggregationTypeTypeDef

```python
# AggregationTypeTypeDef definition

class AggregationTypeTypeDef(TypedDict):
    name: AggregationTypeNameType,  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AggregationTypeNameType](./literals.md#aggregationtypenametype) 
## AlertTargetTypeDef

```python
# AlertTargetTypeDef definition

class AlertTargetTypeDef(TypedDict):
    alertTargetArn: str,
    roleArn: str,
```

## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyArn: NotRequired[str],
```

## AssetPropertyTimestampTypeDef

```python
# AssetPropertyTimestampTypeDef definition

class AssetPropertyTimestampTypeDef(TypedDict):
    timeInSeconds: str,
    offsetInNanos: NotRequired[str],
```

## AssetPropertyVariantTypeDef

```python
# AssetPropertyVariantTypeDef definition

class AssetPropertyVariantTypeDef(TypedDict):
    stringValue: NotRequired[str],
    integerValue: NotRequired[str],
    doubleValue: NotRequired[str],
    booleanValue: NotRequired[str],
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

## AssociateTargetsWithJobRequestRequestTypeDef

```python
# AssociateTargetsWithJobRequestRequestTypeDef definition

class AssociateTargetsWithJobRequestRequestTypeDef(TypedDict):
    targets: Sequence[str],
    jobId: str,
    comment: NotRequired[str],
    namespaceId: NotRequired[str],
```

## AttachPolicyRequestRequestTypeDef

```python
# AttachPolicyRequestRequestTypeDef definition

class AttachPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    target: str,
```

## AttachPrincipalPolicyRequestRequestTypeDef

```python
# AttachPrincipalPolicyRequestRequestTypeDef definition

class AttachPrincipalPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    principal: str,
```

## AttachSecurityProfileRequestRequestTypeDef

```python
# AttachSecurityProfileRequestRequestTypeDef definition

class AttachSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileTargetArn: str,
```

## AttachThingPrincipalRequestRequestTypeDef

```python
# AttachThingPrincipalRequestRequestTypeDef definition

class AttachThingPrincipalRequestRequestTypeDef(TypedDict):
    thingName: str,
    principal: str,
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
## AttributePayloadOutputTypeDef

```python
# AttributePayloadOutputTypeDef definition

class AttributePayloadOutputTypeDef(TypedDict):
    attributes: NotRequired[Dict[str, str]],
    merge: NotRequired[bool],
```

## AttributePayloadTypeDef

```python
# AttributePayloadTypeDef definition

class AttributePayloadTypeDef(TypedDict):
    attributes: NotRequired[Mapping[str, str]],
    merge: NotRequired[bool],
```

## AuditCheckConfigurationTypeDef

```python
# AuditCheckConfigurationTypeDef definition

class AuditCheckConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## AuditCheckDetailsTypeDef

```python
# AuditCheckDetailsTypeDef definition

class AuditCheckDetailsTypeDef(TypedDict):
    checkRunStatus: NotRequired[AuditCheckRunStatusType],  # (1)
    checkCompliant: NotRequired[bool],
    totalResourcesCount: NotRequired[int],
    nonCompliantResourcesCount: NotRequired[int],
    suppressedNonCompliantResourcesCount: NotRequired[int],
    errorCode: NotRequired[str],
    message: NotRequired[str],
```

1. See [:material-code-brackets: AuditCheckRunStatusType](./literals.md#auditcheckrunstatustype) 
## AuditMitigationActionExecutionMetadataTypeDef

```python
# AuditMitigationActionExecutionMetadataTypeDef definition

class AuditMitigationActionExecutionMetadataTypeDef(TypedDict):
    taskId: NotRequired[str],
    findingId: NotRequired[str],
    actionName: NotRequired[str],
    actionId: NotRequired[str],
    status: NotRequired[AuditMitigationActionsExecutionStatusType],  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    errorCode: NotRequired[str],
    message: NotRequired[str],
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype) 
## AuditMitigationActionsTaskMetadataTypeDef

```python
# AuditMitigationActionsTaskMetadataTypeDef definition

class AuditMitigationActionsTaskMetadataTypeDef(TypedDict):
    taskId: NotRequired[str],
    startTime: NotRequired[datetime],
    taskStatus: NotRequired[AuditMitigationActionsTaskStatusType],  # (1)
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
## AuditMitigationActionsTaskTargetOutputTypeDef

```python
# AuditMitigationActionsTaskTargetOutputTypeDef definition

class AuditMitigationActionsTaskTargetOutputTypeDef(TypedDict):
    auditTaskId: NotRequired[str],
    findingIds: NotRequired[List[str]],
    auditCheckToReasonCodeFilter: NotRequired[Dict[str, List[str]]],
```

## AuditMitigationActionsTaskTargetTypeDef

```python
# AuditMitigationActionsTaskTargetTypeDef definition

class AuditMitigationActionsTaskTargetTypeDef(TypedDict):
    auditTaskId: NotRequired[str],
    findingIds: NotRequired[Sequence[str]],
    auditCheckToReasonCodeFilter: NotRequired[Mapping[str, Sequence[str]]],
```

## AuditNotificationTargetTypeDef

```python
# AuditNotificationTargetTypeDef definition

class AuditNotificationTargetTypeDef(TypedDict):
    targetArn: NotRequired[str],
    roleArn: NotRequired[str],
    enabled: NotRequired[bool],
```

## AuditTaskMetadataTypeDef

```python
# AuditTaskMetadataTypeDef definition

class AuditTaskMetadataTypeDef(TypedDict):
    taskId: NotRequired[str],
    taskStatus: NotRequired[AuditTaskStatusType],  # (1)
    taskType: NotRequired[AuditTaskTypeType],  # (2)
```

1. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
2. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
## AuthInfoOutputTypeDef

```python
# AuthInfoOutputTypeDef definition

class AuthInfoOutputTypeDef(TypedDict):
    resources: List[str],
    actionType: NotRequired[ActionTypeType],  # (1)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## AuthInfoTypeDef

```python
# AuthInfoTypeDef definition

class AuthInfoTypeDef(TypedDict):
    resources: Sequence[str],
    actionType: NotRequired[ActionTypeType],  # (1)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## AuthorizerConfigTypeDef

```python
# AuthorizerConfigTypeDef definition

class AuthorizerConfigTypeDef(TypedDict):
    defaultAuthorizerName: NotRequired[str],
    allowAuthorizerOverride: NotRequired[bool],
```

## AuthorizerDescriptionTypeDef

```python
# AuthorizerDescriptionTypeDef definition

class AuthorizerDescriptionTypeDef(TypedDict):
    authorizerName: NotRequired[str],
    authorizerArn: NotRequired[str],
    authorizerFunctionArn: NotRequired[str],
    tokenKeyName: NotRequired[str],
    tokenSigningPublicKeys: NotRequired[Dict[str, str]],
    status: NotRequired[AuthorizerStatusType],  # (1)
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
    signingDisabled: NotRequired[bool],
    enableCachingForHttp: NotRequired[bool],
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
## AuthorizerSummaryTypeDef

```python
# AuthorizerSummaryTypeDef definition

class AuthorizerSummaryTypeDef(TypedDict):
    authorizerName: NotRequired[str],
    authorizerArn: NotRequired[str],
```

## AwsJobAbortCriteriaTypeDef

```python
# AwsJobAbortCriteriaTypeDef definition

class AwsJobAbortCriteriaTypeDef(TypedDict):
    failureType: AwsJobAbortCriteriaFailureTypeType,  # (1)
    action: AwsJobAbortCriteriaAbortActionType,  # (2)
    thresholdPercentage: float,
    minNumberOfExecutedThings: int,
```

1. See [:material-code-brackets: AwsJobAbortCriteriaFailureTypeType](./literals.md#awsjobabortcriteriafailuretypetype) 
2. See [:material-code-brackets: AwsJobAbortCriteriaAbortActionType](./literals.md#awsjobabortcriteriaabortactiontype) 
## AwsJobRateIncreaseCriteriaTypeDef

```python
# AwsJobRateIncreaseCriteriaTypeDef definition

class AwsJobRateIncreaseCriteriaTypeDef(TypedDict):
    numberOfNotifiedThings: NotRequired[int],
    numberOfSucceededThings: NotRequired[int],
```

## AwsJobPresignedUrlConfigTypeDef

```python
# AwsJobPresignedUrlConfigTypeDef definition

class AwsJobPresignedUrlConfigTypeDef(TypedDict):
    expiresInSec: NotRequired[int],
```

## AwsJobTimeoutConfigTypeDef

```python
# AwsJobTimeoutConfigTypeDef definition

class AwsJobTimeoutConfigTypeDef(TypedDict):
    inProgressTimeoutInMinutes: NotRequired[int],
```

## MachineLearningDetectionConfigTypeDef

```python
# MachineLearningDetectionConfigTypeDef definition

class MachineLearningDetectionConfigTypeDef(TypedDict):
    confidenceLevel: ConfidenceLevelType,  # (1)
```

1. See [:material-code-brackets: ConfidenceLevelType](./literals.md#confidenceleveltype) 
## StatisticalThresholdTypeDef

```python
# StatisticalThresholdTypeDef definition

class StatisticalThresholdTypeDef(TypedDict):
    statistic: NotRequired[str],
```

## BehaviorModelTrainingSummaryTypeDef

```python
# BehaviorModelTrainingSummaryTypeDef definition

class BehaviorModelTrainingSummaryTypeDef(TypedDict):
    securityProfileName: NotRequired[str],
    behaviorName: NotRequired[str],
    trainingDataCollectionStartDate: NotRequired[datetime],
    modelStatus: NotRequired[ModelStatusType],  # (1)
    datapointsCollectionPercentage: NotRequired[float],
    lastModelRefreshDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    dimensionName: str,
    operator: NotRequired[DimensionValueOperatorType],  # (1)
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype) 
## BillingGroupMetadataTypeDef

```python
# BillingGroupMetadataTypeDef definition

class BillingGroupMetadataTypeDef(TypedDict):
    creationDate: NotRequired[datetime],
```

## BillingGroupPropertiesTypeDef

```python
# BillingGroupPropertiesTypeDef definition

class BillingGroupPropertiesTypeDef(TypedDict):
    billingGroupDescription: NotRequired[str],
```

## BucketTypeDef

```python
# BucketTypeDef definition

class BucketTypeDef(TypedDict):
    keyValue: NotRequired[str],
    count: NotRequired[int],
```

## TermsAggregationTypeDef

```python
# TermsAggregationTypeDef definition

class TermsAggregationTypeDef(TypedDict):
    maxBuckets: NotRequired[int],
```

## CertificateValidityTypeDef

```python
# CertificateValidityTypeDef definition

class CertificateValidityTypeDef(TypedDict):
    notBefore: NotRequired[datetime],
    notAfter: NotRequired[datetime],
```

## CACertificateTypeDef

```python
# CACertificateTypeDef definition

class CACertificateTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateId: NotRequired[str],
    status: NotRequired[CACertificateStatusType],  # (1)
    creationDate: NotRequired[datetime],
```

1. See [:material-code-brackets: CACertificateStatusType](./literals.md#cacertificatestatustype) 
## CancelAuditMitigationActionsTaskRequestRequestTypeDef

```python
# CancelAuditMitigationActionsTaskRequestRequestTypeDef definition

class CancelAuditMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## CancelAuditTaskRequestRequestTypeDef

```python
# CancelAuditTaskRequestRequestTypeDef definition

class CancelAuditTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## CancelCertificateTransferRequestRequestTypeDef

```python
# CancelCertificateTransferRequestRequestTypeDef definition

class CancelCertificateTransferRequestRequestTypeDef(TypedDict):
    certificateId: str,
```

## CancelDetectMitigationActionsTaskRequestRequestTypeDef

```python
# CancelDetectMitigationActionsTaskRequestRequestTypeDef definition

class CancelDetectMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## CancelJobExecutionRequestRequestTypeDef

```python
# CancelJobExecutionRequestRequestTypeDef definition

class CancelJobExecutionRequestRequestTypeDef(TypedDict):
    jobId: str,
    thingName: str,
    force: NotRequired[bool],
    expectedVersion: NotRequired[int],
    statusDetails: NotRequired[Mapping[str, str]],
```

## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    reasonCode: NotRequired[str],
    comment: NotRequired[str],
    force: NotRequired[bool],
```

## TransferDataTypeDef

```python
# TransferDataTypeDef definition

class TransferDataTypeDef(TypedDict):
    transferMessage: NotRequired[str],
    rejectReason: NotRequired[str],
    transferDate: NotRequired[datetime],
    acceptDate: NotRequired[datetime],
    rejectDate: NotRequired[datetime],
```

## CertificateProviderSummaryTypeDef

```python
# CertificateProviderSummaryTypeDef definition

class CertificateProviderSummaryTypeDef(TypedDict):
    certificateProviderName: NotRequired[str],
    certificateProviderArn: NotRequired[str],
```

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateId: NotRequired[str],
    status: NotRequired[CertificateStatusType],  # (1)
    certificateMode: NotRequired[CertificateModeType],  # (2)
    creationDate: NotRequired[datetime],
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-brackets: CertificateModeType](./literals.md#certificatemodetype) 
## ClientCertificateConfigTypeDef

```python
# ClientCertificateConfigTypeDef definition

class ClientCertificateConfigTypeDef(TypedDict):
    clientCertificateCallbackArn: NotRequired[str],
```

## CodeSigningCertificateChainTypeDef

```python
# CodeSigningCertificateChainTypeDef definition

class CodeSigningCertificateChainTypeDef(TypedDict):
    certificateName: NotRequired[str],
    inlineDocument: NotRequired[str],
```

## CodeSigningSignatureOutputTypeDef

```python
# CodeSigningSignatureOutputTypeDef definition

class CodeSigningSignatureOutputTypeDef(TypedDict):
    inlineDocument: NotRequired[bytes],
```

## CommandExecutionResultTypeDef

```python
# CommandExecutionResultTypeDef definition

class CommandExecutionResultTypeDef(TypedDict):
    S: NotRequired[str],
    B: NotRequired[bool],
    BIN: NotRequired[bytes],
```

## CommandExecutionSummaryTypeDef

```python
# CommandExecutionSummaryTypeDef definition

class CommandExecutionSummaryTypeDef(TypedDict):
    commandArn: NotRequired[str],
    executionId: NotRequired[str],
    targetArn: NotRequired[str],
    status: NotRequired[CommandExecutionStatusType],  # (1)
    createdAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    completedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype) 
## CommandParameterValueOutputTypeDef

```python
# CommandParameterValueOutputTypeDef definition

class CommandParameterValueOutputTypeDef(TypedDict):
    S: NotRequired[str],
    B: NotRequired[bool],
    I: NotRequired[int],
    L: NotRequired[int],
    D: NotRequired[float],
    BIN: NotRequired[bytes],
    UL: NotRequired[str],
```

## CommandPayloadOutputTypeDef

```python
# CommandPayloadOutputTypeDef definition

class CommandPayloadOutputTypeDef(TypedDict):
    content: NotRequired[bytes],
    contentType: NotRequired[str],
```

## CommandSummaryTypeDef

```python
# CommandSummaryTypeDef definition

class CommandSummaryTypeDef(TypedDict):
    commandArn: NotRequired[str],
    commandId: NotRequired[str],
    displayName: NotRequired[str],
    deprecated: NotRequired[bool],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    pendingDeletion: NotRequired[bool],
```

## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## ConfirmTopicRuleDestinationRequestRequestTypeDef

```python
# ConfirmTopicRuleDestinationRequestRequestTypeDef definition

class ConfirmTopicRuleDestinationRequestRequestTypeDef(TypedDict):
    confirmationToken: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## CreateCertificateFromCsrRequestRequestTypeDef

```python
# CreateCertificateFromCsrRequestRequestTypeDef definition

class CreateCertificateFromCsrRequestRequestTypeDef(TypedDict):
    certificateSigningRequest: str,
    setAsActive: NotRequired[bool],
```

## ServerCertificateConfigTypeDef

```python
# ServerCertificateConfigTypeDef definition

class ServerCertificateConfigTypeDef(TypedDict):
    enableOCSPCheck: NotRequired[bool],
    ocspLambdaArn: NotRequired[str],
    ocspAuthorizedResponderArn: NotRequired[str],
```

## TlsConfigTypeDef

```python
# TlsConfigTypeDef definition

class TlsConfigTypeDef(TypedDict):
    securityPolicy: NotRequired[str],
```

## PresignedUrlConfigTypeDef

```python
# PresignedUrlConfigTypeDef definition

class PresignedUrlConfigTypeDef(TypedDict):
    roleArn: NotRequired[str],
    expiresInSec: NotRequired[int],
```

## TimeoutConfigTypeDef

```python
# TimeoutConfigTypeDef definition

class TimeoutConfigTypeDef(TypedDict):
    inProgressTimeoutInMinutes: NotRequired[int],
```

## MaintenanceWindowTypeDef

```python
# MaintenanceWindowTypeDef definition

class MaintenanceWindowTypeDef(TypedDict):
    startTime: str,
    durationInMinutes: int,
```

## CreateKeysAndCertificateRequestRequestTypeDef

```python
# CreateKeysAndCertificateRequestRequestTypeDef definition

class CreateKeysAndCertificateRequestRequestTypeDef(TypedDict):
    setAsActive: NotRequired[bool],
```

## KeyPairTypeDef

```python
# KeyPairTypeDef definition

class KeyPairTypeDef(TypedDict):
    PublicKey: NotRequired[str],
    PrivateKey: NotRequired[str],
```

## CreatePackageRequestRequestTypeDef

```python
# CreatePackageRequestRequestTypeDef definition

class CreatePackageRequestRequestTypeDef(TypedDict):
    packageName: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## CreatePolicyVersionRequestRequestTypeDef

```python
# CreatePolicyVersionRequestRequestTypeDef definition

class CreatePolicyVersionRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyDocument: str,
    setAsDefault: NotRequired[bool],
```

## CreateProvisioningClaimRequestRequestTypeDef

```python
# CreateProvisioningClaimRequestRequestTypeDef definition

class CreateProvisioningClaimRequestRequestTypeDef(TypedDict):
    templateName: str,
```

## ProvisioningHookTypeDef

```python
# ProvisioningHookTypeDef definition

class ProvisioningHookTypeDef(TypedDict):
    targetArn: str,
    payloadVersion: NotRequired[str],
```

## CreateProvisioningTemplateVersionRequestRequestTypeDef

```python
# CreateProvisioningTemplateVersionRequestRequestTypeDef definition

class CreateProvisioningTemplateVersionRequestRequestTypeDef(TypedDict):
    templateName: str,
    templateBody: str,
    setAsDefault: NotRequired[bool],
```

## MetricsExportConfigTypeDef

```python
# MetricsExportConfigTypeDef definition

class MetricsExportConfigTypeDef(TypedDict):
    mqttTopic: str,
    roleArn: str,
```

## DeleteAccountAuditConfigurationRequestRequestTypeDef

```python
# DeleteAccountAuditConfigurationRequestRequestTypeDef definition

class DeleteAccountAuditConfigurationRequestRequestTypeDef(TypedDict):
    deleteScheduledAudits: NotRequired[bool],
```

## DeleteAuthorizerRequestRequestTypeDef

```python
# DeleteAuthorizerRequestRequestTypeDef definition

class DeleteAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
```

## DeleteBillingGroupRequestRequestTypeDef

```python
# DeleteBillingGroupRequestRequestTypeDef definition

class DeleteBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: str,
    expectedVersion: NotRequired[int],
```

## DeleteCACertificateRequestRequestTypeDef

```python
# DeleteCACertificateRequestRequestTypeDef definition

class DeleteCACertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
```

## DeleteCertificateProviderRequestRequestTypeDef

```python
# DeleteCertificateProviderRequestRequestTypeDef definition

class DeleteCertificateProviderRequestRequestTypeDef(TypedDict):
    certificateProviderName: str,
```

## DeleteCertificateRequestRequestTypeDef

```python
# DeleteCertificateRequestRequestTypeDef definition

class DeleteCertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
    forceDelete: NotRequired[bool],
```

## DeleteCommandExecutionRequestRequestTypeDef

```python
# DeleteCommandExecutionRequestRequestTypeDef definition

class DeleteCommandExecutionRequestRequestTypeDef(TypedDict):
    executionId: str,
    targetArn: str,
```

## DeleteCommandRequestRequestTypeDef

```python
# DeleteCommandRequestRequestTypeDef definition

class DeleteCommandRequestRequestTypeDef(TypedDict):
    commandId: str,
```

## DeleteCustomMetricRequestRequestTypeDef

```python
# DeleteCustomMetricRequestRequestTypeDef definition

class DeleteCustomMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
```

## DeleteDimensionRequestRequestTypeDef

```python
# DeleteDimensionRequestRequestTypeDef definition

class DeleteDimensionRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteDomainConfigurationRequestRequestTypeDef

```python
# DeleteDomainConfigurationRequestRequestTypeDef definition

class DeleteDomainConfigurationRequestRequestTypeDef(TypedDict):
    domainConfigurationName: str,
```

## DeleteDynamicThingGroupRequestRequestTypeDef

```python
# DeleteDynamicThingGroupRequestRequestTypeDef definition

class DeleteDynamicThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    expectedVersion: NotRequired[int],
```

## DeleteFleetMetricRequestRequestTypeDef

```python
# DeleteFleetMetricRequestRequestTypeDef definition

class DeleteFleetMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
    expectedVersion: NotRequired[int],
```

## DeleteJobExecutionRequestRequestTypeDef

```python
# DeleteJobExecutionRequestRequestTypeDef definition

class DeleteJobExecutionRequestRequestTypeDef(TypedDict):
    jobId: str,
    thingName: str,
    executionNumber: int,
    force: NotRequired[bool],
    namespaceId: NotRequired[str],
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    force: NotRequired[bool],
    namespaceId: NotRequired[str],
```

## DeleteJobTemplateRequestRequestTypeDef

```python
# DeleteJobTemplateRequestRequestTypeDef definition

class DeleteJobTemplateRequestRequestTypeDef(TypedDict):
    jobTemplateId: str,
```

## DeleteMitigationActionRequestRequestTypeDef

```python
# DeleteMitigationActionRequestRequestTypeDef definition

class DeleteMitigationActionRequestRequestTypeDef(TypedDict):
    actionName: str,
```

## DeleteOTAUpdateRequestRequestTypeDef

```python
# DeleteOTAUpdateRequestRequestTypeDef definition

class DeleteOTAUpdateRequestRequestTypeDef(TypedDict):
    otaUpdateId: str,
    deleteStream: NotRequired[bool],
    forceDeleteAWSJob: NotRequired[bool],
```

## DeletePackageRequestRequestTypeDef

```python
# DeletePackageRequestRequestTypeDef definition

class DeletePackageRequestRequestTypeDef(TypedDict):
    packageName: str,
    clientToken: NotRequired[str],
```

## DeletePackageVersionRequestRequestTypeDef

```python
# DeletePackageVersionRequestRequestTypeDef definition

class DeletePackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    clientToken: NotRequired[str],
```

## DeletePolicyRequestRequestTypeDef

```python
# DeletePolicyRequestRequestTypeDef definition

class DeletePolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
```

## DeletePolicyVersionRequestRequestTypeDef

```python
# DeletePolicyVersionRequestRequestTypeDef definition

class DeletePolicyVersionRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyVersionId: str,
```

## DeleteProvisioningTemplateRequestRequestTypeDef

```python
# DeleteProvisioningTemplateRequestRequestTypeDef definition

class DeleteProvisioningTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
```

## DeleteProvisioningTemplateVersionRequestRequestTypeDef

```python
# DeleteProvisioningTemplateVersionRequestRequestTypeDef definition

class DeleteProvisioningTemplateVersionRequestRequestTypeDef(TypedDict):
    templateName: str,
    versionId: int,
```

## DeleteRoleAliasRequestRequestTypeDef

```python
# DeleteRoleAliasRequestRequestTypeDef definition

class DeleteRoleAliasRequestRequestTypeDef(TypedDict):
    roleAlias: str,
```

## DeleteScheduledAuditRequestRequestTypeDef

```python
# DeleteScheduledAuditRequestRequestTypeDef definition

class DeleteScheduledAuditRequestRequestTypeDef(TypedDict):
    scheduledAuditName: str,
```

## DeleteSecurityProfileRequestRequestTypeDef

```python
# DeleteSecurityProfileRequestRequestTypeDef definition

class DeleteSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    expectedVersion: NotRequired[int],
```

## DeleteStreamRequestRequestTypeDef

```python
# DeleteStreamRequestRequestTypeDef definition

class DeleteStreamRequestRequestTypeDef(TypedDict):
    streamId: str,
```

## DeleteThingGroupRequestRequestTypeDef

```python
# DeleteThingGroupRequestRequestTypeDef definition

class DeleteThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    expectedVersion: NotRequired[int],
```

## DeleteThingRequestRequestTypeDef

```python
# DeleteThingRequestRequestTypeDef definition

class DeleteThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    expectedVersion: NotRequired[int],
```

## DeleteThingTypeRequestRequestTypeDef

```python
# DeleteThingTypeRequestRequestTypeDef definition

class DeleteThingTypeRequestRequestTypeDef(TypedDict):
    thingTypeName: str,
```

## DeleteTopicRuleDestinationRequestRequestTypeDef

```python
# DeleteTopicRuleDestinationRequestRequestTypeDef definition

class DeleteTopicRuleDestinationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteTopicRuleRequestRequestTypeDef

```python
# DeleteTopicRuleRequestRequestTypeDef definition

class DeleteTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
```

## DeleteV2LoggingLevelRequestRequestTypeDef

```python
# DeleteV2LoggingLevelRequestRequestTypeDef definition

class DeleteV2LoggingLevelRequestRequestTypeDef(TypedDict):
    targetType: LogTargetTypeType,  # (1)
    targetName: str,
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
## DeprecateThingTypeRequestRequestTypeDef

```python
# DeprecateThingTypeRequestRequestTypeDef definition

class DeprecateThingTypeRequestRequestTypeDef(TypedDict):
    thingTypeName: str,
    undoDeprecate: NotRequired[bool],
```

## DescribeAuditFindingRequestRequestTypeDef

```python
# DescribeAuditFindingRequestRequestTypeDef definition

class DescribeAuditFindingRequestRequestTypeDef(TypedDict):
    findingId: str,
```

## DescribeAuditMitigationActionsTaskRequestRequestTypeDef

```python
# DescribeAuditMitigationActionsTaskRequestRequestTypeDef definition

class DescribeAuditMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## TaskStatisticsForAuditCheckTypeDef

```python
# TaskStatisticsForAuditCheckTypeDef definition

class TaskStatisticsForAuditCheckTypeDef(TypedDict):
    totalFindingsCount: NotRequired[int],
    failedFindingsCount: NotRequired[int],
    succeededFindingsCount: NotRequired[int],
    skippedFindingsCount: NotRequired[int],
    canceledFindingsCount: NotRequired[int],
```

## DescribeAuditTaskRequestRequestTypeDef

```python
# DescribeAuditTaskRequestRequestTypeDef definition

class DescribeAuditTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## TaskStatisticsTypeDef

```python
# TaskStatisticsTypeDef definition

class TaskStatisticsTypeDef(TypedDict):
    totalChecks: NotRequired[int],
    inProgressChecks: NotRequired[int],
    waitingForDataCollectionChecks: NotRequired[int],
    compliantChecks: NotRequired[int],
    nonCompliantChecks: NotRequired[int],
    failedChecks: NotRequired[int],
    canceledChecks: NotRequired[int],
```

## DescribeAuthorizerRequestRequestTypeDef

```python
# DescribeAuthorizerRequestRequestTypeDef definition

class DescribeAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
```

## DescribeBillingGroupRequestRequestTypeDef

```python
# DescribeBillingGroupRequestRequestTypeDef definition

class DescribeBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: str,
```

## DescribeCACertificateRequestRequestTypeDef

```python
# DescribeCACertificateRequestRequestTypeDef definition

class DescribeCACertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
```

## RegistrationConfigTypeDef

```python
# RegistrationConfigTypeDef definition

class RegistrationConfigTypeDef(TypedDict):
    templateBody: NotRequired[str],
    roleArn: NotRequired[str],
    templateName: NotRequired[str],
```

## DescribeCertificateProviderRequestRequestTypeDef

```python
# DescribeCertificateProviderRequestRequestTypeDef definition

class DescribeCertificateProviderRequestRequestTypeDef(TypedDict):
    certificateProviderName: str,
```

## DescribeCertificateRequestRequestTypeDef

```python
# DescribeCertificateRequestRequestTypeDef definition

class DescribeCertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
```

## DescribeCustomMetricRequestRequestTypeDef

```python
# DescribeCustomMetricRequestRequestTypeDef definition

class DescribeCustomMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
```

## DescribeDetectMitigationActionsTaskRequestRequestTypeDef

```python
# DescribeDetectMitigationActionsTaskRequestRequestTypeDef definition

class DescribeDetectMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## DescribeDimensionRequestRequestTypeDef

```python
# DescribeDimensionRequestRequestTypeDef definition

class DescribeDimensionRequestRequestTypeDef(TypedDict):
    name: str,
```

## DescribeDomainConfigurationRequestRequestTypeDef

```python
# DescribeDomainConfigurationRequestRequestTypeDef definition

class DescribeDomainConfigurationRequestRequestTypeDef(TypedDict):
    domainConfigurationName: str,
```

## ServerCertificateSummaryTypeDef

```python
# ServerCertificateSummaryTypeDef definition

class ServerCertificateSummaryTypeDef(TypedDict):
    serverCertificateArn: NotRequired[str],
    serverCertificateStatus: NotRequired[ServerCertificateStatusType],  # (1)
    serverCertificateStatusDetail: NotRequired[str],
```

1. See [:material-code-brackets: ServerCertificateStatusType](./literals.md#servercertificatestatustype) 
## DescribeEndpointRequestRequestTypeDef

```python
# DescribeEndpointRequestRequestTypeDef definition

class DescribeEndpointRequestRequestTypeDef(TypedDict):
    endpointType: NotRequired[str],
```

## DescribeFleetMetricRequestRequestTypeDef

```python
# DescribeFleetMetricRequestRequestTypeDef definition

class DescribeFleetMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
```

## DescribeIndexRequestRequestTypeDef

```python
# DescribeIndexRequestRequestTypeDef definition

class DescribeIndexRequestRequestTypeDef(TypedDict):
    indexName: str,
```

## DescribeJobExecutionRequestRequestTypeDef

```python
# DescribeJobExecutionRequestRequestTypeDef definition

class DescribeJobExecutionRequestRequestTypeDef(TypedDict):
    jobId: str,
    thingName: str,
    executionNumber: NotRequired[int],
```

## DescribeJobRequestRequestTypeDef

```python
# DescribeJobRequestRequestTypeDef definition

class DescribeJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    beforeSubstitution: NotRequired[bool],
```

## DescribeJobTemplateRequestRequestTypeDef

```python
# DescribeJobTemplateRequestRequestTypeDef definition

class DescribeJobTemplateRequestRequestTypeDef(TypedDict):
    jobTemplateId: str,
```

## DescribeManagedJobTemplateRequestRequestTypeDef

```python
# DescribeManagedJobTemplateRequestRequestTypeDef definition

class DescribeManagedJobTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
    templateVersion: NotRequired[str],
```

## DocumentParameterTypeDef

```python
# DocumentParameterTypeDef definition

class DocumentParameterTypeDef(TypedDict):
    key: NotRequired[str],
    description: NotRequired[str],
    regex: NotRequired[str],
    example: NotRequired[str],
    optional: NotRequired[bool],
```

## DescribeMitigationActionRequestRequestTypeDef

```python
# DescribeMitigationActionRequestRequestTypeDef definition

class DescribeMitigationActionRequestRequestTypeDef(TypedDict):
    actionName: str,
```

## DescribeProvisioningTemplateRequestRequestTypeDef

```python
# DescribeProvisioningTemplateRequestRequestTypeDef definition

class DescribeProvisioningTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
```

## DescribeProvisioningTemplateVersionRequestRequestTypeDef

```python
# DescribeProvisioningTemplateVersionRequestRequestTypeDef definition

class DescribeProvisioningTemplateVersionRequestRequestTypeDef(TypedDict):
    templateName: str,
    versionId: int,
```

## DescribeRoleAliasRequestRequestTypeDef

```python
# DescribeRoleAliasRequestRequestTypeDef definition

class DescribeRoleAliasRequestRequestTypeDef(TypedDict):
    roleAlias: str,
```

## RoleAliasDescriptionTypeDef

```python
# RoleAliasDescriptionTypeDef definition

class RoleAliasDescriptionTypeDef(TypedDict):
    roleAlias: NotRequired[str],
    roleAliasArn: NotRequired[str],
    roleArn: NotRequired[str],
    owner: NotRequired[str],
    credentialDurationSeconds: NotRequired[int],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
```

## DescribeScheduledAuditRequestRequestTypeDef

```python
# DescribeScheduledAuditRequestRequestTypeDef definition

class DescribeScheduledAuditRequestRequestTypeDef(TypedDict):
    scheduledAuditName: str,
```

## DescribeSecurityProfileRequestRequestTypeDef

```python
# DescribeSecurityProfileRequestRequestTypeDef definition

class DescribeSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
```

## DescribeStreamRequestRequestTypeDef

```python
# DescribeStreamRequestRequestTypeDef definition

class DescribeStreamRequestRequestTypeDef(TypedDict):
    streamId: str,
```

## DescribeThingGroupRequestRequestTypeDef

```python
# DescribeThingGroupRequestRequestTypeDef definition

class DescribeThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
```

## DescribeThingRegistrationTaskRequestRequestTypeDef

```python
# DescribeThingRegistrationTaskRequestRequestTypeDef definition

class DescribeThingRegistrationTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## DescribeThingRequestRequestTypeDef

```python
# DescribeThingRequestRequestTypeDef definition

class DescribeThingRequestRequestTypeDef(TypedDict):
    thingName: str,
```

## DescribeThingTypeRequestRequestTypeDef

```python
# DescribeThingTypeRequestRequestTypeDef definition

class DescribeThingTypeRequestRequestTypeDef(TypedDict):
    thingTypeName: str,
```

## ThingTypeMetadataTypeDef

```python
# ThingTypeMetadataTypeDef definition

class ThingTypeMetadataTypeDef(TypedDict):
    deprecated: NotRequired[bool],
    deprecationDate: NotRequired[datetime],
    creationDate: NotRequired[datetime],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## DetachPolicyRequestRequestTypeDef

```python
# DetachPolicyRequestRequestTypeDef definition

class DetachPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    target: str,
```

## DetachPrincipalPolicyRequestRequestTypeDef

```python
# DetachPrincipalPolicyRequestRequestTypeDef definition

class DetachPrincipalPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    principal: str,
```

## DetachSecurityProfileRequestRequestTypeDef

```python
# DetachSecurityProfileRequestRequestTypeDef definition

class DetachSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileTargetArn: str,
```

## DetachThingPrincipalRequestRequestTypeDef

```python
# DetachThingPrincipalRequestRequestTypeDef definition

class DetachThingPrincipalRequestRequestTypeDef(TypedDict):
    thingName: str,
    principal: str,
```

## DetectMitigationActionExecutionTypeDef

```python
# DetectMitigationActionExecutionTypeDef definition

class DetectMitigationActionExecutionTypeDef(TypedDict):
    taskId: NotRequired[str],
    violationId: NotRequired[str],
    actionName: NotRequired[str],
    thingName: NotRequired[str],
    executionStartDate: NotRequired[datetime],
    executionEndDate: NotRequired[datetime],
    status: NotRequired[DetectMitigationActionExecutionStatusType],  # (1)
    errorCode: NotRequired[str],
    message: NotRequired[str],
```

1. See [:material-code-brackets: DetectMitigationActionExecutionStatusType](./literals.md#detectmitigationactionexecutionstatustype) 
## DetectMitigationActionsTaskStatisticsTypeDef

```python
# DetectMitigationActionsTaskStatisticsTypeDef definition

class DetectMitigationActionsTaskStatisticsTypeDef(TypedDict):
    actionsExecuted: NotRequired[int],
    actionsSkipped: NotRequired[int],
    actionsFailed: NotRequired[int],
```

## DetectMitigationActionsTaskTargetOutputTypeDef

```python
# DetectMitigationActionsTaskTargetOutputTypeDef definition

class DetectMitigationActionsTaskTargetOutputTypeDef(TypedDict):
    violationIds: NotRequired[List[str]],
    securityProfileName: NotRequired[str],
    behaviorName: NotRequired[str],
```

## ViolationEventOccurrenceRangeOutputTypeDef

```python
# ViolationEventOccurrenceRangeOutputTypeDef definition

class ViolationEventOccurrenceRangeOutputTypeDef(TypedDict):
    startTime: datetime,
    endTime: datetime,
```

## DetectMitigationActionsTaskTargetTypeDef

```python
# DetectMitigationActionsTaskTargetTypeDef definition

class DetectMitigationActionsTaskTargetTypeDef(TypedDict):
    violationIds: NotRequired[Sequence[str]],
    securityProfileName: NotRequired[str],
    behaviorName: NotRequired[str],
```

## DisableTopicRuleRequestRequestTypeDef

```python
# DisableTopicRuleRequestRequestTypeDef definition

class DisableTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
```

## DisassociateSbomFromPackageVersionRequestRequestTypeDef

```python
# DisassociateSbomFromPackageVersionRequestRequestTypeDef definition

class DisassociateSbomFromPackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    clientToken: NotRequired[str],
```

## DomainConfigurationSummaryTypeDef

```python
# DomainConfigurationSummaryTypeDef definition

class DomainConfigurationSummaryTypeDef(TypedDict):
    domainConfigurationName: NotRequired[str],
    domainConfigurationArn: NotRequired[str],
    serviceType: NotRequired[ServiceTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## PutItemInputTypeDef

```python
# PutItemInputTypeDef definition

class PutItemInputTypeDef(TypedDict):
    tableName: str,
```

## EffectivePolicyTypeDef

```python
# EffectivePolicyTypeDef definition

class EffectivePolicyTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyArn: NotRequired[str],
    policyDocument: NotRequired[str],
```

## EnableIoTLoggingParamsTypeDef

```python
# EnableIoTLoggingParamsTypeDef definition

class EnableIoTLoggingParamsTypeDef(TypedDict):
    roleArnForLogging: str,
    logLevel: LogLevelType,  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## EnableTopicRuleRequestRequestTypeDef

```python
# EnableTopicRuleRequestRequestTypeDef definition

class EnableTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
```

## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## RateIncreaseCriteriaTypeDef

```python
# RateIncreaseCriteriaTypeDef definition

class RateIncreaseCriteriaTypeDef(TypedDict):
    numberOfNotifiedThings: NotRequired[int],
    numberOfSucceededThings: NotRequired[int],
```

## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[FieldTypeType],  # (1)
```

1. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    version: NotRequired[str],
```

## StreamTypeDef

```python
# StreamTypeDef definition

class StreamTypeDef(TypedDict):
    streamId: NotRequired[str],
    fileId: NotRequired[int],
```

## FleetMetricNameAndArnTypeDef

```python
# FleetMetricNameAndArnTypeDef definition

class FleetMetricNameAndArnTypeDef(TypedDict):
    metricName: NotRequired[str],
    metricArn: NotRequired[str],
```

## GeoLocationTargetTypeDef

```python
# GeoLocationTargetTypeDef definition

class GeoLocationTargetTypeDef(TypedDict):
    name: NotRequired[str],
    order: NotRequired[TargetFieldOrderType],  # (1)
```

1. See [:material-code-brackets: TargetFieldOrderType](./literals.md#targetfieldordertype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetBehaviorModelTrainingSummariesRequestRequestTypeDef

```python
# GetBehaviorModelTrainingSummariesRequestRequestTypeDef definition

class GetBehaviorModelTrainingSummariesRequestRequestTypeDef(TypedDict):
    securityProfileName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetCardinalityRequestRequestTypeDef

```python
# GetCardinalityRequestRequestTypeDef definition

class GetCardinalityRequestRequestTypeDef(TypedDict):
    queryString: str,
    indexName: NotRequired[str],
    aggregationField: NotRequired[str],
    queryVersion: NotRequired[str],
```

## GetCommandExecutionRequestRequestTypeDef

```python
# GetCommandExecutionRequestRequestTypeDef definition

class GetCommandExecutionRequestRequestTypeDef(TypedDict):
    executionId: str,
    targetArn: str,
    includeResult: NotRequired[bool],
```

## StatusReasonTypeDef

```python
# StatusReasonTypeDef definition

class StatusReasonTypeDef(TypedDict):
    reasonCode: str,
    reasonDescription: NotRequired[str],
```

## GetCommandRequestRequestTypeDef

```python
# GetCommandRequestRequestTypeDef definition

class GetCommandRequestRequestTypeDef(TypedDict):
    commandId: str,
```

## GetEffectivePoliciesRequestRequestTypeDef

```python
# GetEffectivePoliciesRequestRequestTypeDef definition

class GetEffectivePoliciesRequestRequestTypeDef(TypedDict):
    principal: NotRequired[str],
    cognitoIdentityPoolId: NotRequired[str],
    thingName: NotRequired[str],
```

## GetJobDocumentRequestRequestTypeDef

```python
# GetJobDocumentRequestRequestTypeDef definition

class GetJobDocumentRequestRequestTypeDef(TypedDict):
    jobId: str,
    beforeSubstitution: NotRequired[bool],
```

## GetOTAUpdateRequestRequestTypeDef

```python
# GetOTAUpdateRequestRequestTypeDef definition

class GetOTAUpdateRequestRequestTypeDef(TypedDict):
    otaUpdateId: str,
```

## VersionUpdateByJobsConfigTypeDef

```python
# VersionUpdateByJobsConfigTypeDef definition

class VersionUpdateByJobsConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
    roleArn: NotRequired[str],
```

## GetPackageRequestRequestTypeDef

```python
# GetPackageRequestRequestTypeDef definition

class GetPackageRequestRequestTypeDef(TypedDict):
    packageName: str,
```

## GetPackageVersionRequestRequestTypeDef

```python
# GetPackageVersionRequestRequestTypeDef definition

class GetPackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
```

## GetPercentilesRequestRequestTypeDef

```python
# GetPercentilesRequestRequestTypeDef definition

class GetPercentilesRequestRequestTypeDef(TypedDict):
    queryString: str,
    indexName: NotRequired[str],
    aggregationField: NotRequired[str],
    queryVersion: NotRequired[str],
    percents: NotRequired[Sequence[float]],
```

## PercentPairTypeDef

```python
# PercentPairTypeDef definition

class PercentPairTypeDef(TypedDict):
    percent: NotRequired[float],
    value: NotRequired[float],
```

## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
```

## GetPolicyVersionRequestRequestTypeDef

```python
# GetPolicyVersionRequestRequestTypeDef definition

class GetPolicyVersionRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyVersionId: str,
```

## GetStatisticsRequestRequestTypeDef

```python
# GetStatisticsRequestRequestTypeDef definition

class GetStatisticsRequestRequestTypeDef(TypedDict):
    queryString: str,
    indexName: NotRequired[str],
    aggregationField: NotRequired[str],
    queryVersion: NotRequired[str],
```

## StatisticsTypeDef

```python
# StatisticsTypeDef definition

class StatisticsTypeDef(TypedDict):
    count: NotRequired[int],
    average: NotRequired[float],
    sum: NotRequired[float],
    minimum: NotRequired[float],
    maximum: NotRequired[float],
    sumOfSquares: NotRequired[float],
    variance: NotRequired[float],
    stdDeviation: NotRequired[float],
```

## GetThingConnectivityDataRequestRequestTypeDef

```python
# GetThingConnectivityDataRequestRequestTypeDef definition

class GetThingConnectivityDataRequestRequestTypeDef(TypedDict):
    thingName: str,
```

## GetTopicRuleDestinationRequestRequestTypeDef

```python
# GetTopicRuleDestinationRequestRequestTypeDef definition

class GetTopicRuleDestinationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetTopicRuleRequestRequestTypeDef

```python
# GetTopicRuleRequestRequestTypeDef definition

class GetTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
```

## GroupNameAndArnTypeDef

```python
# GroupNameAndArnTypeDef definition

class GroupNameAndArnTypeDef(TypedDict):
    groupName: NotRequired[str],
    groupArn: NotRequired[str],
```

## HttpActionHeaderTypeDef

```python
# HttpActionHeaderTypeDef definition

class HttpActionHeaderTypeDef(TypedDict):
    key: str,
    value: str,
```

## SigV4AuthorizationTypeDef

```python
# SigV4AuthorizationTypeDef definition

class SigV4AuthorizationTypeDef(TypedDict):
    signingRegion: str,
    serviceName: str,
    roleArn: str,
```

## HttpContextTypeDef

```python
# HttpContextTypeDef definition

class HttpContextTypeDef(TypedDict):
    headers: NotRequired[Mapping[str, str]],
    queryString: NotRequired[str],
```

## HttpUrlDestinationConfigurationTypeDef

```python
# HttpUrlDestinationConfigurationTypeDef definition

class HttpUrlDestinationConfigurationTypeDef(TypedDict):
    confirmationUrl: str,
```

## HttpUrlDestinationPropertiesTypeDef

```python
# HttpUrlDestinationPropertiesTypeDef definition

class HttpUrlDestinationPropertiesTypeDef(TypedDict):
    confirmationUrl: NotRequired[str],
```

## HttpUrlDestinationSummaryTypeDef

```python
# HttpUrlDestinationSummaryTypeDef definition

class HttpUrlDestinationSummaryTypeDef(TypedDict):
    confirmationUrl: NotRequired[str],
```

## IssuerCertificateIdentifierTypeDef

```python
# IssuerCertificateIdentifierTypeDef definition

class IssuerCertificateIdentifierTypeDef(TypedDict):
    issuerCertificateSubject: NotRequired[str],
    issuerId: NotRequired[str],
    issuerCertificateSerialNumber: NotRequired[str],
```

## JobExecutionStatusDetailsTypeDef

```python
# JobExecutionStatusDetailsTypeDef definition

class JobExecutionStatusDetailsTypeDef(TypedDict):
    detailsMap: NotRequired[Dict[str, str]],
```

## JobExecutionSummaryTypeDef

```python
# JobExecutionSummaryTypeDef definition

class JobExecutionSummaryTypeDef(TypedDict):
    status: NotRequired[JobExecutionStatusType],  # (1)
    queuedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    executionNumber: NotRequired[int],
    retryAttempt: NotRequired[int],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
## RetryCriteriaTypeDef

```python
# RetryCriteriaTypeDef definition

class RetryCriteriaTypeDef(TypedDict):
    failureType: RetryableFailureTypeType,  # (1)
    numberOfRetries: int,
```

1. See [:material-code-brackets: RetryableFailureTypeType](./literals.md#retryablefailuretypetype) 
## JobProcessDetailsTypeDef

```python
# JobProcessDetailsTypeDef definition

class JobProcessDetailsTypeDef(TypedDict):
    processingTargets: NotRequired[List[str]],
    numberOfCanceledThings: NotRequired[int],
    numberOfSucceededThings: NotRequired[int],
    numberOfFailedThings: NotRequired[int],
    numberOfRejectedThings: NotRequired[int],
    numberOfQueuedThings: NotRequired[int],
    numberOfInProgressThings: NotRequired[int],
    numberOfRemovedThings: NotRequired[int],
    numberOfTimedOutThings: NotRequired[int],
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobArn: NotRequired[str],
    jobId: NotRequired[str],
    thingGroupId: NotRequired[str],
    targetSelection: NotRequired[TargetSelectionType],  # (1)
    status: NotRequired[JobStatusType],  # (2)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    completedAt: NotRequired[datetime],
    isConcurrent: NotRequired[bool],
```

1. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## JobTemplateSummaryTypeDef

```python
# JobTemplateSummaryTypeDef definition

class JobTemplateSummaryTypeDef(TypedDict):
    jobTemplateArn: NotRequired[str],
    jobTemplateId: NotRequired[str],
    description: NotRequired[str],
    createdAt: NotRequired[datetime],
```

## ScheduledJobRolloutTypeDef

```python
# ScheduledJobRolloutTypeDef definition

class ScheduledJobRolloutTypeDef(TypedDict):
    startTime: NotRequired[str],
```

## KafkaActionHeaderTypeDef

```python
# KafkaActionHeaderTypeDef definition

class KafkaActionHeaderTypeDef(TypedDict):
    key: str,
    value: str,
```

## ListActiveViolationsRequestRequestTypeDef

```python
# ListActiveViolationsRequestRequestTypeDef definition

class ListActiveViolationsRequestRequestTypeDef(TypedDict):
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behaviorCriteriaType: NotRequired[BehaviorCriteriaTypeType],  # (1)
    listSuppressedAlerts: NotRequired[bool],
    verificationState: NotRequired[VerificationStateType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
## ListAttachedPoliciesRequestRequestTypeDef

```python
# ListAttachedPoliciesRequestRequestTypeDef definition

class ListAttachedPoliciesRequestRequestTypeDef(TypedDict):
    target: str,
    recursive: NotRequired[bool],
    marker: NotRequired[str],
    pageSize: NotRequired[int],
```

## ListAuditMitigationActionsExecutionsRequestRequestTypeDef

```python
# ListAuditMitigationActionsExecutionsRequestRequestTypeDef definition

class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(TypedDict):
    taskId: str,
    findingId: str,
    actionStatus: NotRequired[AuditMitigationActionsExecutionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype) 
## ListAuthorizersRequestRequestTypeDef

```python
# ListAuthorizersRequestRequestTypeDef definition

class ListAuthorizersRequestRequestTypeDef(TypedDict):
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
    status: NotRequired[AuthorizerStatusType],  # (1)
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
## ListBillingGroupsRequestRequestTypeDef

```python
# ListBillingGroupsRequestRequestTypeDef definition

class ListBillingGroupsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    namePrefixFilter: NotRequired[str],
```

## ListCACertificatesRequestRequestTypeDef

```python
# ListCACertificatesRequestRequestTypeDef definition

class ListCACertificatesRequestRequestTypeDef(TypedDict):
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
    templateName: NotRequired[str],
```

## ListCertificateProvidersRequestRequestTypeDef

```python
# ListCertificateProvidersRequestRequestTypeDef definition

class ListCertificateProvidersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## ListCertificatesByCARequestRequestTypeDef

```python
# ListCertificatesByCARequestRequestTypeDef definition

class ListCertificatesByCARequestRequestTypeDef(TypedDict):
    caCertificateId: str,
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## ListCertificatesRequestRequestTypeDef

```python
# ListCertificatesRequestRequestTypeDef definition

class ListCertificatesRequestRequestTypeDef(TypedDict):
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## TimeFilterTypeDef

```python
# TimeFilterTypeDef definition

class TimeFilterTypeDef(TypedDict):
    after: NotRequired[str],
    before: NotRequired[str],
```

## ListCommandsRequestRequestTypeDef

```python
# ListCommandsRequestRequestTypeDef definition

class ListCommandsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    namespace: NotRequired[CommandNamespaceType],  # (1)
    commandParameterName: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListCustomMetricsRequestRequestTypeDef

```python
# ListCustomMetricsRequestRequestTypeDef definition

class ListCustomMetricsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDimensionsRequestRequestTypeDef

```python
# ListDimensionsRequestRequestTypeDef definition

class ListDimensionsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDomainConfigurationsRequestRequestTypeDef

```python
# ListDomainConfigurationsRequestRequestTypeDef definition

class ListDomainConfigurationsRequestRequestTypeDef(TypedDict):
    marker: NotRequired[str],
    pageSize: NotRequired[int],
    serviceType: NotRequired[ServiceTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListFleetMetricsRequestRequestTypeDef

```python
# ListFleetMetricsRequestRequestTypeDef definition

class ListFleetMetricsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListIndicesRequestRequestTypeDef

```python
# ListIndicesRequestRequestTypeDef definition

class ListIndicesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobExecutionsForJobRequestRequestTypeDef

```python
# ListJobExecutionsForJobRequestRequestTypeDef definition

class ListJobExecutionsForJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    status: NotRequired[JobExecutionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
## ListJobExecutionsForThingRequestRequestTypeDef

```python
# ListJobExecutionsForThingRequestRequestTypeDef definition

class ListJobExecutionsForThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    status: NotRequired[JobExecutionStatusType],  # (1)
    namespaceId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    jobId: NotRequired[str],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
## ListJobTemplatesRequestRequestTypeDef

```python
# ListJobTemplatesRequestRequestTypeDef definition

class ListJobTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    status: NotRequired[JobStatusType],  # (1)
    targetSelection: NotRequired[TargetSelectionType],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    thingGroupName: NotRequired[str],
    thingGroupId: NotRequired[str],
    namespaceId: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
## ListManagedJobTemplatesRequestRequestTypeDef

```python
# ListManagedJobTemplatesRequestRequestTypeDef definition

class ListManagedJobTemplatesRequestRequestTypeDef(TypedDict):
    templateName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedJobTemplateSummaryTypeDef

```python
# ManagedJobTemplateSummaryTypeDef definition

class ManagedJobTemplateSummaryTypeDef(TypedDict):
    templateArn: NotRequired[str],
    templateName: NotRequired[str],
    description: NotRequired[str],
    environments: NotRequired[List[str]],
    templateVersion: NotRequired[str],
```

## ListMitigationActionsRequestRequestTypeDef

```python
# ListMitigationActionsRequestRequestTypeDef definition

class ListMitigationActionsRequestRequestTypeDef(TypedDict):
    actionType: NotRequired[MitigationActionTypeType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype) 
## MitigationActionIdentifierTypeDef

```python
# MitigationActionIdentifierTypeDef definition

class MitigationActionIdentifierTypeDef(TypedDict):
    actionName: NotRequired[str],
    actionArn: NotRequired[str],
    creationDate: NotRequired[datetime],
```

## ListOTAUpdatesRequestRequestTypeDef

```python
# ListOTAUpdatesRequestRequestTypeDef definition

class ListOTAUpdatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    otaUpdateStatus: NotRequired[OTAUpdateStatusType],  # (1)
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
## OTAUpdateSummaryTypeDef

```python
# OTAUpdateSummaryTypeDef definition

class OTAUpdateSummaryTypeDef(TypedDict):
    otaUpdateId: NotRequired[str],
    otaUpdateArn: NotRequired[str],
    creationDate: NotRequired[datetime],
```

## ListOutgoingCertificatesRequestRequestTypeDef

```python
# ListOutgoingCertificatesRequestRequestTypeDef definition

class ListOutgoingCertificatesRequestRequestTypeDef(TypedDict):
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## OutgoingCertificateTypeDef

```python
# OutgoingCertificateTypeDef definition

class OutgoingCertificateTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateId: NotRequired[str],
    transferredTo: NotRequired[str],
    transferDate: NotRequired[datetime],
    transferMessage: NotRequired[str],
    creationDate: NotRequired[datetime],
```

## ListPackageVersionsRequestRequestTypeDef

```python
# ListPackageVersionsRequestRequestTypeDef definition

class ListPackageVersionsRequestRequestTypeDef(TypedDict):
    packageName: str,
    status: NotRequired[PackageVersionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## PackageVersionSummaryTypeDef

```python
# PackageVersionSummaryTypeDef definition

class PackageVersionSummaryTypeDef(TypedDict):
    packageName: NotRequired[str],
    versionName: NotRequired[str],
    status: NotRequired[PackageVersionStatusType],  # (1)
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## ListPackagesRequestRequestTypeDef

```python
# ListPackagesRequestRequestTypeDef definition

class ListPackagesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PackageSummaryTypeDef

```python
# PackageSummaryTypeDef definition

class PackageSummaryTypeDef(TypedDict):
    packageName: NotRequired[str],
    defaultVersionName: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
```

## ListPoliciesRequestRequestTypeDef

```python
# ListPoliciesRequestRequestTypeDef definition

class ListPoliciesRequestRequestTypeDef(TypedDict):
    marker: NotRequired[str],
    pageSize: NotRequired[int],
    ascendingOrder: NotRequired[bool],
```

## ListPolicyPrincipalsRequestRequestTypeDef

```python
# ListPolicyPrincipalsRequestRequestTypeDef definition

class ListPolicyPrincipalsRequestRequestTypeDef(TypedDict):
    policyName: str,
    marker: NotRequired[str],
    pageSize: NotRequired[int],
    ascendingOrder: NotRequired[bool],
```

## ListPolicyVersionsRequestRequestTypeDef

```python
# ListPolicyVersionsRequestRequestTypeDef definition

class ListPolicyVersionsRequestRequestTypeDef(TypedDict):
    policyName: str,
```

## PolicyVersionTypeDef

```python
# PolicyVersionTypeDef definition

class PolicyVersionTypeDef(TypedDict):
    versionId: NotRequired[str],
    isDefaultVersion: NotRequired[bool],
    createDate: NotRequired[datetime],
```

## ListPrincipalPoliciesRequestRequestTypeDef

```python
# ListPrincipalPoliciesRequestRequestTypeDef definition

class ListPrincipalPoliciesRequestRequestTypeDef(TypedDict):
    principal: str,
    marker: NotRequired[str],
    pageSize: NotRequired[int],
    ascendingOrder: NotRequired[bool],
```

## ListPrincipalThingsRequestRequestTypeDef

```python
# ListPrincipalThingsRequestRequestTypeDef definition

class ListPrincipalThingsRequestRequestTypeDef(TypedDict):
    principal: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPrincipalThingsV2RequestRequestTypeDef

```python
# ListPrincipalThingsV2RequestRequestTypeDef definition

class ListPrincipalThingsV2RequestRequestTypeDef(TypedDict):
    principal: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
## PrincipalThingObjectTypeDef

```python
# PrincipalThingObjectTypeDef definition

class PrincipalThingObjectTypeDef(TypedDict):
    thingName: str,
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
## ListProvisioningTemplateVersionsRequestRequestTypeDef

```python
# ListProvisioningTemplateVersionsRequestRequestTypeDef definition

class ListProvisioningTemplateVersionsRequestRequestTypeDef(TypedDict):
    templateName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProvisioningTemplateVersionSummaryTypeDef

```python
# ProvisioningTemplateVersionSummaryTypeDef definition

class ProvisioningTemplateVersionSummaryTypeDef(TypedDict):
    versionId: NotRequired[int],
    creationDate: NotRequired[datetime],
    isDefaultVersion: NotRequired[bool],
```

## ListProvisioningTemplatesRequestRequestTypeDef

```python
# ListProvisioningTemplatesRequestRequestTypeDef definition

class ListProvisioningTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProvisioningTemplateSummaryTypeDef

```python
# ProvisioningTemplateSummaryTypeDef definition

class ProvisioningTemplateSummaryTypeDef(TypedDict):
    templateArn: NotRequired[str],
    templateName: NotRequired[str],
    description: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
    enabled: NotRequired[bool],
    type: NotRequired[TemplateTypeType],  # (1)
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## ListRelatedResourcesForAuditFindingRequestRequestTypeDef

```python
# ListRelatedResourcesForAuditFindingRequestRequestTypeDef definition

class ListRelatedResourcesForAuditFindingRequestRequestTypeDef(TypedDict):
    findingId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListRoleAliasesRequestRequestTypeDef

```python
# ListRoleAliasesRequestRequestTypeDef definition

class ListRoleAliasesRequestRequestTypeDef(TypedDict):
    pageSize: NotRequired[int],
    marker: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## ListSbomValidationResultsRequestRequestTypeDef

```python
# ListSbomValidationResultsRequestRequestTypeDef definition

class ListSbomValidationResultsRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    validationResult: NotRequired[SbomValidationResultType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SbomValidationResultType](./literals.md#sbomvalidationresulttype) 
## SbomValidationResultSummaryTypeDef

```python
# SbomValidationResultSummaryTypeDef definition

class SbomValidationResultSummaryTypeDef(TypedDict):
    fileName: NotRequired[str],
    validationResult: NotRequired[SbomValidationResultType],  # (1)
    errorCode: NotRequired[SbomValidationErrorCodeType],  # (2)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: SbomValidationResultType](./literals.md#sbomvalidationresulttype) 
2. See [:material-code-brackets: SbomValidationErrorCodeType](./literals.md#sbomvalidationerrorcodetype) 
## ListScheduledAuditsRequestRequestTypeDef

```python
# ListScheduledAuditsRequestRequestTypeDef definition

class ListScheduledAuditsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ScheduledAuditMetadataTypeDef

```python
# ScheduledAuditMetadataTypeDef definition

class ScheduledAuditMetadataTypeDef(TypedDict):
    scheduledAuditName: NotRequired[str],
    scheduledAuditArn: NotRequired[str],
    frequency: NotRequired[AuditFrequencyType],  # (1)
    dayOfMonth: NotRequired[str],
    dayOfWeek: NotRequired[DayOfWeekType],  # (2)
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
## ListSecurityProfilesForTargetRequestRequestTypeDef

```python
# ListSecurityProfilesForTargetRequestRequestTypeDef definition

class ListSecurityProfilesForTargetRequestRequestTypeDef(TypedDict):
    securityProfileTargetArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    recursive: NotRequired[bool],
```

## ListSecurityProfilesRequestRequestTypeDef

```python
# ListSecurityProfilesRequestRequestTypeDef definition

class ListSecurityProfilesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    dimensionName: NotRequired[str],
    metricName: NotRequired[str],
```

## SecurityProfileIdentifierTypeDef

```python
# SecurityProfileIdentifierTypeDef definition

class SecurityProfileIdentifierTypeDef(TypedDict):
    name: str,
    arn: str,
```

## ListStreamsRequestRequestTypeDef

```python
# ListStreamsRequestRequestTypeDef definition

class ListStreamsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    ascendingOrder: NotRequired[bool],
```

## StreamSummaryTypeDef

```python
# StreamSummaryTypeDef definition

class StreamSummaryTypeDef(TypedDict):
    streamId: NotRequired[str],
    streamArn: NotRequired[str],
    streamVersion: NotRequired[int],
    description: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    nextToken: NotRequired[str],
```

## ListTargetsForPolicyRequestRequestTypeDef

```python
# ListTargetsForPolicyRequestRequestTypeDef definition

class ListTargetsForPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    marker: NotRequired[str],
    pageSize: NotRequired[int],
```

## ListTargetsForSecurityProfileRequestRequestTypeDef

```python
# ListTargetsForSecurityProfileRequestRequestTypeDef definition

class ListTargetsForSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SecurityProfileTargetTypeDef

```python
# SecurityProfileTargetTypeDef definition

class SecurityProfileTargetTypeDef(TypedDict):
    arn: str,
```

## ListThingGroupsForThingRequestRequestTypeDef

```python
# ListThingGroupsForThingRequestRequestTypeDef definition

class ListThingGroupsForThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListThingGroupsRequestRequestTypeDef

```python
# ListThingGroupsRequestRequestTypeDef definition

class ListThingGroupsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    parentGroup: NotRequired[str],
    namePrefixFilter: NotRequired[str],
    recursive: NotRequired[bool],
```

## ListThingPrincipalsRequestRequestTypeDef

```python
# ListThingPrincipalsRequestRequestTypeDef definition

class ListThingPrincipalsRequestRequestTypeDef(TypedDict):
    thingName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListThingPrincipalsV2RequestRequestTypeDef

```python
# ListThingPrincipalsV2RequestRequestTypeDef definition

class ListThingPrincipalsV2RequestRequestTypeDef(TypedDict):
    thingName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
## ThingPrincipalObjectTypeDef

```python
# ThingPrincipalObjectTypeDef definition

class ThingPrincipalObjectTypeDef(TypedDict):
    principal: str,
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
## ListThingRegistrationTaskReportsRequestRequestTypeDef

```python
# ListThingRegistrationTaskReportsRequestRequestTypeDef definition

class ListThingRegistrationTaskReportsRequestRequestTypeDef(TypedDict):
    taskId: str,
    reportType: ReportTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
## ListThingRegistrationTasksRequestRequestTypeDef

```python
# ListThingRegistrationTasksRequestRequestTypeDef definition

class ListThingRegistrationTasksRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ListThingTypesRequestRequestTypeDef

```python
# ListThingTypesRequestRequestTypeDef definition

class ListThingTypesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    thingTypeName: NotRequired[str],
```

## ListThingsInBillingGroupRequestRequestTypeDef

```python
# ListThingsInBillingGroupRequestRequestTypeDef definition

class ListThingsInBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListThingsInThingGroupRequestRequestTypeDef

```python
# ListThingsInThingGroupRequestRequestTypeDef definition

class ListThingsInThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    recursive: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListThingsRequestRequestTypeDef

```python
# ListThingsRequestRequestTypeDef definition

class ListThingsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    thingTypeName: NotRequired[str],
    usePrefixAttributeValue: NotRequired[bool],
```

## ThingAttributeTypeDef

```python
# ThingAttributeTypeDef definition

class ThingAttributeTypeDef(TypedDict):
    thingName: NotRequired[str],
    thingTypeName: NotRequired[str],
    thingArn: NotRequired[str],
    attributes: NotRequired[Dict[str, str]],
    version: NotRequired[int],
```

## ListTopicRuleDestinationsRequestRequestTypeDef

```python
# ListTopicRuleDestinationsRequestRequestTypeDef definition

class ListTopicRuleDestinationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTopicRulesRequestRequestTypeDef

```python
# ListTopicRulesRequestRequestTypeDef definition

class ListTopicRulesRequestRequestTypeDef(TypedDict):
    topic: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    ruleDisabled: NotRequired[bool],
```

## TopicRuleListItemTypeDef

```python
# TopicRuleListItemTypeDef definition

class TopicRuleListItemTypeDef(TypedDict):
    ruleArn: NotRequired[str],
    ruleName: NotRequired[str],
    topicPattern: NotRequired[str],
    createdAt: NotRequired[datetime],
    ruleDisabled: NotRequired[bool],
```

## ListV2LoggingLevelsRequestRequestTypeDef

```python
# ListV2LoggingLevelsRequestRequestTypeDef definition

class ListV2LoggingLevelsRequestRequestTypeDef(TypedDict):
    targetType: NotRequired[LogTargetTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
## LocationTimestampTypeDef

```python
# LocationTimestampTypeDef definition

class LocationTimestampTypeDef(TypedDict):
    value: str,
    unit: NotRequired[str],
```

## LogTargetTypeDef

```python
# LogTargetTypeDef definition

class LogTargetTypeDef(TypedDict):
    targetType: LogTargetTypeType,  # (1)
    targetName: NotRequired[str],
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
## LoggingOptionsPayloadTypeDef

```python
# LoggingOptionsPayloadTypeDef definition

class LoggingOptionsPayloadTypeDef(TypedDict):
    roleArn: str,
    logLevel: NotRequired[LogLevelType],  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## MetricValueTypeDef

```python
# MetricValueTypeDef definition

class MetricValueTypeDef(TypedDict):
    count: NotRequired[int],
    cidrs: NotRequired[Sequence[str]],
    ports: NotRequired[Sequence[int]],
    number: NotRequired[float],
    numbers: NotRequired[Sequence[float]],
    strings: NotRequired[Sequence[str]],
```

## PublishFindingToSnsParamsTypeDef

```python
# PublishFindingToSnsParamsTypeDef definition

class PublishFindingToSnsParamsTypeDef(TypedDict):
    topicArn: str,
```

## ReplaceDefaultPolicyVersionParamsTypeDef

```python
# ReplaceDefaultPolicyVersionParamsTypeDef definition

class ReplaceDefaultPolicyVersionParamsTypeDef(TypedDict):
    templateName: PolicyTemplateNameType,  # (1)
```

1. See [:material-code-brackets: PolicyTemplateNameType](./literals.md#policytemplatenametype) 
## UpdateCACertificateParamsTypeDef

```python
# UpdateCACertificateParamsTypeDef definition

class UpdateCACertificateParamsTypeDef(TypedDict):
    action: CACertificateUpdateActionType,  # (1)
```

1. See [:material-code-brackets: CACertificateUpdateActionType](./literals.md#cacertificateupdateactiontype) 
## UpdateDeviceCertificateParamsTypeDef

```python
# UpdateDeviceCertificateParamsTypeDef definition

class UpdateDeviceCertificateParamsTypeDef(TypedDict):
    action: DeviceCertificateUpdateActionType,  # (1)
```

1. See [:material-code-brackets: DeviceCertificateUpdateActionType](./literals.md#devicecertificateupdateactiontype) 
## PropagatingAttributeTypeDef

```python
# PropagatingAttributeTypeDef definition

class PropagatingAttributeTypeDef(TypedDict):
    userPropertyKey: NotRequired[str],
    thingAttribute: NotRequired[str],
    connectionAttribute: NotRequired[str],
```

## UserPropertyTypeDef

```python
# UserPropertyTypeDef definition

class UserPropertyTypeDef(TypedDict):
    key: str,
    value: str,
```

## PolicyVersionIdentifierTypeDef

```python
# PolicyVersionIdentifierTypeDef definition

class PolicyVersionIdentifierTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyVersionId: NotRequired[str],
```

## PutVerificationStateOnViolationRequestRequestTypeDef

```python
# PutVerificationStateOnViolationRequestRequestTypeDef definition

class PutVerificationStateOnViolationRequestRequestTypeDef(TypedDict):
    violationId: str,
    verificationState: VerificationStateType,  # (1)
    verificationStateDescription: NotRequired[str],
```

1. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
## RegisterCertificateRequestRequestTypeDef

```python
# RegisterCertificateRequestRequestTypeDef definition

class RegisterCertificateRequestRequestTypeDef(TypedDict):
    certificatePem: str,
    caCertificatePem: NotRequired[str],
    setAsActive: NotRequired[bool],
    status: NotRequired[CertificateStatusType],  # (1)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
## RegisterCertificateWithoutCARequestRequestTypeDef

```python
# RegisterCertificateWithoutCARequestRequestTypeDef definition

class RegisterCertificateWithoutCARequestRequestTypeDef(TypedDict):
    certificatePem: str,
    status: NotRequired[CertificateStatusType],  # (1)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
## RegisterThingRequestRequestTypeDef

```python
# RegisterThingRequestRequestTypeDef definition

class RegisterThingRequestRequestTypeDef(TypedDict):
    templateBody: str,
    parameters: NotRequired[Mapping[str, str]],
```

## RejectCertificateTransferRequestRequestTypeDef

```python
# RejectCertificateTransferRequestRequestTypeDef definition

class RejectCertificateTransferRequestRequestTypeDef(TypedDict):
    certificateId: str,
    rejectReason: NotRequired[str],
```

## RemoveThingFromBillingGroupRequestRequestTypeDef

```python
# RemoveThingFromBillingGroupRequestRequestTypeDef definition

class RemoveThingFromBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: NotRequired[str],
    billingGroupArn: NotRequired[str],
    thingName: NotRequired[str],
    thingArn: NotRequired[str],
```

## RemoveThingFromThingGroupRequestRequestTypeDef

```python
# RemoveThingFromThingGroupRequestRequestTypeDef definition

class RemoveThingFromThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: NotRequired[str],
    thingGroupArn: NotRequired[str],
    thingName: NotRequired[str],
    thingArn: NotRequired[str],
```

## SearchIndexRequestRequestTypeDef

```python
# SearchIndexRequestRequestTypeDef definition

class SearchIndexRequestRequestTypeDef(TypedDict):
    queryString: str,
    indexName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    queryVersion: NotRequired[str],
```

## ThingGroupDocumentTypeDef

```python
# ThingGroupDocumentTypeDef definition

class ThingGroupDocumentTypeDef(TypedDict):
    thingGroupName: NotRequired[str],
    thingGroupId: NotRequired[str],
    thingGroupDescription: NotRequired[str],
    attributes: NotRequired[Dict[str, str]],
    parentGroupNames: NotRequired[List[str]],
```

## SetDefaultAuthorizerRequestRequestTypeDef

```python
# SetDefaultAuthorizerRequestRequestTypeDef definition

class SetDefaultAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
```

## SetDefaultPolicyVersionRequestRequestTypeDef

```python
# SetDefaultPolicyVersionRequestRequestTypeDef definition

class SetDefaultPolicyVersionRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyVersionId: str,
```

## SetV2LoggingOptionsRequestRequestTypeDef

```python
# SetV2LoggingOptionsRequestRequestTypeDef definition

class SetV2LoggingOptionsRequestRequestTypeDef(TypedDict):
    roleArn: NotRequired[str],
    defaultLogLevel: NotRequired[LogLevelType],  # (1)
    disableAllLogs: NotRequired[bool],
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## SigningProfileParameterTypeDef

```python
# SigningProfileParameterTypeDef definition

class SigningProfileParameterTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    platform: NotRequired[str],
    certificatePathOnDevice: NotRequired[str],
```

## StartOnDemandAuditTaskRequestRequestTypeDef

```python
# StartOnDemandAuditTaskRequestRequestTypeDef definition

class StartOnDemandAuditTaskRequestRequestTypeDef(TypedDict):
    targetCheckNames: Sequence[str],
```

## StartThingRegistrationTaskRequestRequestTypeDef

```python
# StartThingRegistrationTaskRequestRequestTypeDef definition

class StartThingRegistrationTaskRequestRequestTypeDef(TypedDict):
    templateBody: str,
    inputFileBucket: str,
    inputFileKey: str,
    roleArn: str,
```

## StopThingRegistrationTaskRequestRequestTypeDef

```python
# StopThingRegistrationTaskRequestRequestTypeDef definition

class StopThingRegistrationTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## TlsContextTypeDef

```python
# TlsContextTypeDef definition

class TlsContextTypeDef(TypedDict):
    serverName: NotRequired[str],
```

## ThingConnectivityTypeDef

```python
# ThingConnectivityTypeDef definition

class ThingConnectivityTypeDef(TypedDict):
    connected: NotRequired[bool],
    timestamp: NotRequired[int],
    disconnectReason: NotRequired[str],
```

## TimestreamDimensionTypeDef

```python
# TimestreamDimensionTypeDef definition

class TimestreamDimensionTypeDef(TypedDict):
    name: str,
    value: str,
```

## TimestreamTimestampTypeDef

```python
# TimestreamTimestampTypeDef definition

class TimestreamTimestampTypeDef(TypedDict):
    value: str,
    unit: str,
```

## VpcDestinationConfigurationTypeDef

```python
# VpcDestinationConfigurationTypeDef definition

class VpcDestinationConfigurationTypeDef(TypedDict):
    subnetIds: Sequence[str],
    vpcId: str,
    roleArn: str,
    securityGroups: NotRequired[Sequence[str]],
```

## VpcDestinationSummaryTypeDef

```python
# VpcDestinationSummaryTypeDef definition

class VpcDestinationSummaryTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroups: NotRequired[List[str]],
    vpcId: NotRequired[str],
    roleArn: NotRequired[str],
```

## VpcDestinationPropertiesTypeDef

```python
# VpcDestinationPropertiesTypeDef definition

class VpcDestinationPropertiesTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroups: NotRequired[List[str]],
    vpcId: NotRequired[str],
    roleArn: NotRequired[str],
```

## TransferCertificateRequestRequestTypeDef

```python
# TransferCertificateRequestRequestTypeDef definition

class TransferCertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
    targetAwsAccount: str,
    transferMessage: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAuthorizerRequestRequestTypeDef

```python
# UpdateAuthorizerRequestRequestTypeDef definition

class UpdateAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
    authorizerFunctionArn: NotRequired[str],
    tokenKeyName: NotRequired[str],
    tokenSigningPublicKeys: NotRequired[Mapping[str, str]],
    status: NotRequired[AuthorizerStatusType],  # (1)
    enableCachingForHttp: NotRequired[bool],
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
## UpdateCertificateProviderRequestRequestTypeDef

```python
# UpdateCertificateProviderRequestRequestTypeDef definition

class UpdateCertificateProviderRequestRequestTypeDef(TypedDict):
    certificateProviderName: str,
    lambdaFunctionArn: NotRequired[str],
    accountDefaultForOperations: NotRequired[Sequence[CertificateProviderOperationType]],  # (1)
```

1. See [:material-code-brackets: CertificateProviderOperationType](./literals.md#certificateprovideroperationtype) 
## UpdateCertificateRequestRequestTypeDef

```python
# UpdateCertificateRequestRequestTypeDef definition

class UpdateCertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
    newStatus: CertificateStatusType,  # (1)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
## UpdateCommandRequestRequestTypeDef

```python
# UpdateCommandRequestRequestTypeDef definition

class UpdateCommandRequestRequestTypeDef(TypedDict):
    commandId: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
    deprecated: NotRequired[bool],
```

## UpdateCustomMetricRequestRequestTypeDef

```python
# UpdateCustomMetricRequestRequestTypeDef definition

class UpdateCustomMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
    displayName: str,
```

## UpdateDimensionRequestRequestTypeDef

```python
# UpdateDimensionRequestRequestTypeDef definition

class UpdateDimensionRequestRequestTypeDef(TypedDict):
    name: str,
    stringValues: Sequence[str],
```

## UpdatePackageRequestRequestTypeDef

```python
# UpdatePackageRequestRequestTypeDef definition

class UpdatePackageRequestRequestTypeDef(TypedDict):
    packageName: str,
    description: NotRequired[str],
    defaultVersionName: NotRequired[str],
    unsetDefaultVersion: NotRequired[bool],
    clientToken: NotRequired[str],
```

## UpdateRoleAliasRequestRequestTypeDef

```python
# UpdateRoleAliasRequestRequestTypeDef definition

class UpdateRoleAliasRequestRequestTypeDef(TypedDict):
    roleAlias: str,
    roleArn: NotRequired[str],
    credentialDurationSeconds: NotRequired[int],
```

## UpdateScheduledAuditRequestRequestTypeDef

```python
# UpdateScheduledAuditRequestRequestTypeDef definition

class UpdateScheduledAuditRequestRequestTypeDef(TypedDict):
    scheduledAuditName: str,
    frequency: NotRequired[AuditFrequencyType],  # (1)
    dayOfMonth: NotRequired[str],
    dayOfWeek: NotRequired[DayOfWeekType],  # (2)
    targetCheckNames: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
## UpdateThingGroupsForThingRequestRequestTypeDef

```python
# UpdateThingGroupsForThingRequestRequestTypeDef definition

class UpdateThingGroupsForThingRequestRequestTypeDef(TypedDict):
    thingName: NotRequired[str],
    thingGroupsToAdd: NotRequired[Sequence[str]],
    thingGroupsToRemove: NotRequired[Sequence[str]],
    overrideDynamicGroups: NotRequired[bool],
```

## UpdateTopicRuleDestinationRequestRequestTypeDef

```python
# UpdateTopicRuleDestinationRequestRequestTypeDef definition

class UpdateTopicRuleDestinationRequestRequestTypeDef(TypedDict):
    arn: str,
    status: TopicRuleDestinationStatusType,  # (1)
```

1. See [:material-code-brackets: TopicRuleDestinationStatusType](./literals.md#topicruledestinationstatustype) 
## ValidationErrorTypeDef

```python
# ValidationErrorTypeDef definition

class ValidationErrorTypeDef(TypedDict):
    errorMessage: NotRequired[str],
```

## AbortConfigOutputTypeDef

```python
# AbortConfigOutputTypeDef definition

class AbortConfigOutputTypeDef(TypedDict):
    criteriaList: List[AbortCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: AbortCriteriaTypeDef](./type_defs.md#abortcriteriatypedef) 
## AbortConfigTypeDef

```python
# AbortConfigTypeDef definition

class AbortConfigTypeDef(TypedDict):
    criteriaList: Sequence[AbortCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: AbortCriteriaTypeDef](./type_defs.md#abortcriteriatypedef) 
## MetricDatumTypeDef

```python
# MetricDatumTypeDef definition

class MetricDatumTypeDef(TypedDict):
    timestamp: NotRequired[datetime],
    value: NotRequired[MetricValueOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 
## UpdateFleetMetricRequestRequestTypeDef

```python
# UpdateFleetMetricRequestRequestTypeDef definition

class UpdateFleetMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
    indexName: str,
    queryString: NotRequired[str],
    aggregationType: NotRequired[AggregationTypeTypeDef],  # (1)
    period: NotRequired[int],
    aggregationField: NotRequired[str],
    description: NotRequired[str],
    queryVersion: NotRequired[str],
    unit: NotRequired[FleetMetricUnitType],  # (2)
    expectedVersion: NotRequired[int],
```

1. See [:material-code-braces: AggregationTypeTypeDef](./type_defs.md#aggregationtypetypedef) 
2. See [:material-code-brackets: FleetMetricUnitType](./literals.md#fleetmetricunittype) 
## AllowedTypeDef

```python
# AllowedTypeDef definition

class AllowedTypeDef(TypedDict):
    policies: NotRequired[List[PolicyTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
## ExplicitDenyTypeDef

```python
# ExplicitDenyTypeDef definition

class ExplicitDenyTypeDef(TypedDict):
    policies: NotRequired[List[PolicyTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
## ImplicitDenyTypeDef

```python
# ImplicitDenyTypeDef definition

class ImplicitDenyTypeDef(TypedDict):
    policies: NotRequired[List[PolicyTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
## AssetPropertyValueTypeDef

```python
# AssetPropertyValueTypeDef definition

class AssetPropertyValueTypeDef(TypedDict):
    value: AssetPropertyVariantTypeDef,  # (1)
    timestamp: AssetPropertyTimestampTypeDef,  # (2)
    quality: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyVariantTypeDef](./type_defs.md#assetpropertyvarianttypedef) 
2. See [:material-code-braces: AssetPropertyTimestampTypeDef](./type_defs.md#assetpropertytimestamptypedef) 
## AssociateTargetsWithJobResponseTypeDef

```python
# AssociateTargetsWithJobResponseTypeDef definition

class AssociateTargetsWithJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobId: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelJobResponseTypeDef

```python
# CancelJobResponseTypeDef definition

class CancelJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobId: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAuthorizerResponseTypeDef

```python
# CreateAuthorizerResponseTypeDef definition

class CreateAuthorizerResponseTypeDef(TypedDict):
    authorizerName: str,
    authorizerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBillingGroupResponseTypeDef

```python
# CreateBillingGroupResponseTypeDef definition

class CreateBillingGroupResponseTypeDef(TypedDict):
    billingGroupName: str,
    billingGroupArn: str,
    billingGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCertificateFromCsrResponseTypeDef

```python
# CreateCertificateFromCsrResponseTypeDef definition

class CreateCertificateFromCsrResponseTypeDef(TypedDict):
    certificateArn: str,
    certificateId: str,
    certificatePem: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCertificateProviderResponseTypeDef

```python
# CreateCertificateProviderResponseTypeDef definition

class CreateCertificateProviderResponseTypeDef(TypedDict):
    certificateProviderName: str,
    certificateProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCommandResponseTypeDef

```python
# CreateCommandResponseTypeDef definition

class CreateCommandResponseTypeDef(TypedDict):
    commandId: str,
    commandArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomMetricResponseTypeDef

```python
# CreateCustomMetricResponseTypeDef definition

class CreateCustomMetricResponseTypeDef(TypedDict):
    metricName: str,
    metricArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDimensionResponseTypeDef

```python
# CreateDimensionResponseTypeDef definition

class CreateDimensionResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainConfigurationResponseTypeDef

```python
# CreateDomainConfigurationResponseTypeDef definition

class CreateDomainConfigurationResponseTypeDef(TypedDict):
    domainConfigurationName: str,
    domainConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDynamicThingGroupResponseTypeDef

```python
# CreateDynamicThingGroupResponseTypeDef definition

class CreateDynamicThingGroupResponseTypeDef(TypedDict):
    thingGroupName: str,
    thingGroupArn: str,
    thingGroupId: str,
    indexName: str,
    queryString: str,
    queryVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetMetricResponseTypeDef

```python
# CreateFleetMetricResponseTypeDef definition

class CreateFleetMetricResponseTypeDef(TypedDict):
    metricName: str,
    metricArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobId: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobTemplateResponseTypeDef

```python
# CreateJobTemplateResponseTypeDef definition

class CreateJobTemplateResponseTypeDef(TypedDict):
    jobTemplateArn: str,
    jobTemplateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMitigationActionResponseTypeDef

```python
# CreateMitigationActionResponseTypeDef definition

class CreateMitigationActionResponseTypeDef(TypedDict):
    actionArn: str,
    actionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOTAUpdateResponseTypeDef

```python
# CreateOTAUpdateResponseTypeDef definition

class CreateOTAUpdateResponseTypeDef(TypedDict):
    otaUpdateId: str,
    awsIotJobId: str,
    otaUpdateArn: str,
    awsIotJobArn: str,
    otaUpdateStatus: OTAUpdateStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageResponseTypeDef

```python
# CreatePackageResponseTypeDef definition

class CreatePackageResponseTypeDef(TypedDict):
    packageName: str,
    packageArn: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageVersionResponseTypeDef

```python
# CreatePackageVersionResponseTypeDef definition

class CreatePackageVersionResponseTypeDef(TypedDict):
    packageVersionArn: str,
    packageName: str,
    versionName: str,
    description: str,
    attributes: Dict[str, str],
    status: PackageVersionStatusType,  # (1)
    errorReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyResponseTypeDef

```python
# CreatePolicyResponseTypeDef definition

class CreatePolicyResponseTypeDef(TypedDict):
    policyName: str,
    policyArn: str,
    policyDocument: str,
    policyVersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyVersionResponseTypeDef

```python
# CreatePolicyVersionResponseTypeDef definition

class CreatePolicyVersionResponseTypeDef(TypedDict):
    policyArn: str,
    policyDocument: str,
    policyVersionId: str,
    isDefaultVersion: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisioningTemplateResponseTypeDef

```python
# CreateProvisioningTemplateResponseTypeDef definition

class CreateProvisioningTemplateResponseTypeDef(TypedDict):
    templateArn: str,
    templateName: str,
    defaultVersionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisioningTemplateVersionResponseTypeDef

```python
# CreateProvisioningTemplateVersionResponseTypeDef definition

class CreateProvisioningTemplateVersionResponseTypeDef(TypedDict):
    templateArn: str,
    templateName: str,
    versionId: int,
    isDefaultVersion: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoleAliasResponseTypeDef

```python
# CreateRoleAliasResponseTypeDef definition

class CreateRoleAliasResponseTypeDef(TypedDict):
    roleAlias: str,
    roleAliasArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduledAuditResponseTypeDef

```python
# CreateScheduledAuditResponseTypeDef definition

class CreateScheduledAuditResponseTypeDef(TypedDict):
    scheduledAuditArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityProfileResponseTypeDef

```python
# CreateSecurityProfileResponseTypeDef definition

class CreateSecurityProfileResponseTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamResponseTypeDef

```python
# CreateStreamResponseTypeDef definition

class CreateStreamResponseTypeDef(TypedDict):
    streamId: str,
    streamArn: str,
    description: str,
    streamVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThingGroupResponseTypeDef

```python
# CreateThingGroupResponseTypeDef definition

class CreateThingGroupResponseTypeDef(TypedDict):
    thingGroupName: str,
    thingGroupArn: str,
    thingGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThingResponseTypeDef

```python
# CreateThingResponseTypeDef definition

class CreateThingResponseTypeDef(TypedDict):
    thingName: str,
    thingArn: str,
    thingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThingTypeResponseTypeDef

```python
# CreateThingTypeResponseTypeDef definition

class CreateThingTypeResponseTypeDef(TypedDict):
    thingTypeName: str,
    thingTypeArn: str,
    thingTypeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCommandResponseTypeDef

```python
# DeleteCommandResponseTypeDef definition

class DeleteCommandResponseTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCertificateProviderResponseTypeDef

```python
# DescribeCertificateProviderResponseTypeDef definition

class DescribeCertificateProviderResponseTypeDef(TypedDict):
    certificateProviderName: str,
    certificateProviderArn: str,
    lambdaFunctionArn: str,
    accountDefaultForOperations: List[CertificateProviderOperationType],  # (1)
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CertificateProviderOperationType](./literals.md#certificateprovideroperationtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomMetricResponseTypeDef

```python
# DescribeCustomMetricResponseTypeDef definition

class DescribeCustomMetricResponseTypeDef(TypedDict):
    metricName: str,
    metricArn: str,
    metricType: CustomMetricTypeType,  # (1)
    displayName: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomMetricTypeType](./literals.md#custommetrictypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDimensionResponseTypeDef

```python
# DescribeDimensionResponseTypeDef definition

class DescribeDimensionResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    type: DimensionTypeType,  # (1)
    stringValues: List[str],
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointResponseTypeDef

```python
# DescribeEndpointResponseTypeDef definition

class DescribeEndpointResponseTypeDef(TypedDict):
    endpointAddress: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetMetricResponseTypeDef

```python
# DescribeFleetMetricResponseTypeDef definition

class DescribeFleetMetricResponseTypeDef(TypedDict):
    metricName: str,
    queryString: str,
    aggregationType: AggregationTypeOutputTypeDef,  # (1)
    period: int,
    aggregationField: str,
    description: str,
    queryVersion: str,
    indexName: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    unit: FleetMetricUnitType,  # (2)
    version: int,
    metricArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AggregationTypeOutputTypeDef](./type_defs.md#aggregationtypeoutputtypedef) 
2. See [:material-code-brackets: FleetMetricUnitType](./literals.md#fleetmetricunittype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIndexResponseTypeDef

```python
# DescribeIndexResponseTypeDef definition

class DescribeIndexResponseTypeDef(TypedDict):
    indexName: str,
    indexStatus: IndexStatusType,  # (1)
    schema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProvisioningTemplateVersionResponseTypeDef

```python
# DescribeProvisioningTemplateVersionResponseTypeDef definition

class DescribeProvisioningTemplateVersionResponseTypeDef(TypedDict):
    versionId: int,
    creationDate: datetime,
    templateBody: str,
    isDefaultVersion: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScheduledAuditResponseTypeDef

```python
# DescribeScheduledAuditResponseTypeDef definition

class DescribeScheduledAuditResponseTypeDef(TypedDict):
    frequency: AuditFrequencyType,  # (1)
    dayOfMonth: str,
    dayOfWeek: DayOfWeekType,  # (2)
    targetCheckNames: List[str],
    scheduledAuditName: str,
    scheduledAuditArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThingRegistrationTaskResponseTypeDef

```python
# DescribeThingRegistrationTaskResponseTypeDef definition

class DescribeThingRegistrationTaskResponseTypeDef(TypedDict):
    taskId: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    templateBody: str,
    inputFileBucket: str,
    inputFileKey: str,
    roleArn: str,
    status: StatusType,  # (1)
    message: str,
    successCount: int,
    failureCount: int,
    percentageProgress: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThingResponseTypeDef

```python
# DescribeThingResponseTypeDef definition

class DescribeThingResponseTypeDef(TypedDict):
    defaultClientId: str,
    thingName: str,
    thingId: str,
    thingArn: str,
    thingTypeName: str,
    attributes: Dict[str, str],
    version: int,
    billingGroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCardinalityResponseTypeDef

```python
# GetCardinalityResponseTypeDef definition

class GetCardinalityResponseTypeDef(TypedDict):
    cardinality: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobDocumentResponseTypeDef

```python
# GetJobDocumentResponseTypeDef definition

class GetJobDocumentResponseTypeDef(TypedDict):
    document: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoggingOptionsResponseTypeDef

```python
# GetLoggingOptionsResponseTypeDef definition

class GetLoggingOptionsResponseTypeDef(TypedDict):
    roleArn: str,
    logLevel: LogLevelType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPackageResponseTypeDef

```python
# GetPackageResponseTypeDef definition

class GetPackageResponseTypeDef(TypedDict):
    packageName: str,
    packageArn: str,
    description: str,
    defaultVersionName: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    policyName: str,
    policyArn: str,
    policyDocument: str,
    defaultVersionId: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    generationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyVersionResponseTypeDef

```python
# GetPolicyVersionResponseTypeDef definition

class GetPolicyVersionResponseTypeDef(TypedDict):
    policyArn: str,
    policyName: str,
    policyDocument: str,
    policyVersionId: str,
    isDefaultVersion: bool,
    creationDate: datetime,
    lastModifiedDate: datetime,
    generationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegistrationCodeResponseTypeDef

```python
# GetRegistrationCodeResponseTypeDef definition

class GetRegistrationCodeResponseTypeDef(TypedDict):
    registrationCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThingConnectivityDataResponseTypeDef

```python
# GetThingConnectivityDataResponseTypeDef definition

class GetThingConnectivityDataResponseTypeDef(TypedDict):
    thingName: str,
    connected: bool,
    timestamp: datetime,
    disconnectReason: DisconnectReasonValueType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DisconnectReasonValueType](./literals.md#disconnectreasonvaluetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetV2LoggingOptionsResponseTypeDef

```python
# GetV2LoggingOptionsResponseTypeDef definition

class GetV2LoggingOptionsResponseTypeDef(TypedDict):
    roleArn: str,
    defaultLogLevel: LogLevelType,  # (1)
    disableAllLogs: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttachedPoliciesResponseTypeDef

```python
# ListAttachedPoliciesResponseTypeDef definition

class ListAttachedPoliciesResponseTypeDef(TypedDict):
    policies: List[PolicyTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomMetricsResponseTypeDef

```python
# ListCustomMetricsResponseTypeDef definition

class ListCustomMetricsResponseTypeDef(TypedDict):
    metricNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDimensionsResponseTypeDef

```python
# ListDimensionsResponseTypeDef definition

class ListDimensionsResponseTypeDef(TypedDict):
    dimensionNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndicesResponseTypeDef

```python
# ListIndicesResponseTypeDef definition

class ListIndicesResponseTypeDef(TypedDict):
    indexNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesResponseTypeDef

```python
# ListPoliciesResponseTypeDef definition

class ListPoliciesResponseTypeDef(TypedDict):
    policies: List[PolicyTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyPrincipalsResponseTypeDef

```python
# ListPolicyPrincipalsResponseTypeDef definition

class ListPolicyPrincipalsResponseTypeDef(TypedDict):
    principals: List[str],
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrincipalPoliciesResponseTypeDef

```python
# ListPrincipalPoliciesResponseTypeDef definition

class ListPrincipalPoliciesResponseTypeDef(TypedDict):
    policies: List[PolicyTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrincipalThingsResponseTypeDef

```python
# ListPrincipalThingsResponseTypeDef definition

class ListPrincipalThingsResponseTypeDef(TypedDict):
    things: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoleAliasesResponseTypeDef

```python
# ListRoleAliasesResponseTypeDef definition

class ListRoleAliasesResponseTypeDef(TypedDict):
    roleAliases: List[str],
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsForPolicyResponseTypeDef

```python
# ListTargetsForPolicyResponseTypeDef definition

class ListTargetsForPolicyResponseTypeDef(TypedDict):
    targets: List[str],
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingPrincipalsResponseTypeDef

```python
# ListThingPrincipalsResponseTypeDef definition

class ListThingPrincipalsResponseTypeDef(TypedDict):
    principals: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingRegistrationTaskReportsResponseTypeDef

```python
# ListThingRegistrationTaskReportsResponseTypeDef definition

class ListThingRegistrationTaskReportsResponseTypeDef(TypedDict):
    resourceLinks: List[str],
    reportType: ReportTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingRegistrationTasksResponseTypeDef

```python
# ListThingRegistrationTasksResponseTypeDef definition

class ListThingRegistrationTasksResponseTypeDef(TypedDict):
    taskIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingsInBillingGroupResponseTypeDef

```python
# ListThingsInBillingGroupResponseTypeDef definition

class ListThingsInBillingGroupResponseTypeDef(TypedDict):
    things: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingsInThingGroupResponseTypeDef

```python
# ListThingsInThingGroupResponseTypeDef definition

class ListThingsInThingGroupResponseTypeDef(TypedDict):
    things: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterCACertificateResponseTypeDef

```python
# RegisterCACertificateResponseTypeDef definition

class RegisterCACertificateResponseTypeDef(TypedDict):
    certificateArn: str,
    certificateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterCertificateResponseTypeDef

```python
# RegisterCertificateResponseTypeDef definition

class RegisterCertificateResponseTypeDef(TypedDict):
    certificateArn: str,
    certificateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterCertificateWithoutCAResponseTypeDef

```python
# RegisterCertificateWithoutCAResponseTypeDef definition

class RegisterCertificateWithoutCAResponseTypeDef(TypedDict):
    certificateArn: str,
    certificateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterThingResponseTypeDef

```python
# RegisterThingResponseTypeDef definition

class RegisterThingResponseTypeDef(TypedDict):
    certificatePem: str,
    resourceArns: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDefaultAuthorizerResponseTypeDef

```python
# SetDefaultAuthorizerResponseTypeDef definition

class SetDefaultAuthorizerResponseTypeDef(TypedDict):
    authorizerName: str,
    authorizerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAuditMitigationActionsTaskResponseTypeDef

```python
# StartAuditMitigationActionsTaskResponseTypeDef definition

class StartAuditMitigationActionsTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDetectMitigationActionsTaskResponseTypeDef

```python
# StartDetectMitigationActionsTaskResponseTypeDef definition

class StartDetectMitigationActionsTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOnDemandAuditTaskResponseTypeDef

```python
# StartOnDemandAuditTaskResponseTypeDef definition

class StartOnDemandAuditTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartThingRegistrationTaskResponseTypeDef

```python
# StartThingRegistrationTaskResponseTypeDef definition

class StartThingRegistrationTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestInvokeAuthorizerResponseTypeDef

```python
# TestInvokeAuthorizerResponseTypeDef definition

class TestInvokeAuthorizerResponseTypeDef(TypedDict):
    isAuthenticated: bool,
    principalId: str,
    policyDocuments: List[str],
    refreshAfterInSeconds: int,
    disconnectAfterInSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferCertificateResponseTypeDef

```python
# TransferCertificateResponseTypeDef definition

class TransferCertificateResponseTypeDef(TypedDict):
    transferredCertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAuthorizerResponseTypeDef

```python
# UpdateAuthorizerResponseTypeDef definition

class UpdateAuthorizerResponseTypeDef(TypedDict):
    authorizerName: str,
    authorizerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillingGroupResponseTypeDef

```python
# UpdateBillingGroupResponseTypeDef definition

class UpdateBillingGroupResponseTypeDef(TypedDict):
    version: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCertificateProviderResponseTypeDef

```python
# UpdateCertificateProviderResponseTypeDef definition

class UpdateCertificateProviderResponseTypeDef(TypedDict):
    certificateProviderName: str,
    certificateProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCommandResponseTypeDef

```python
# UpdateCommandResponseTypeDef definition

class UpdateCommandResponseTypeDef(TypedDict):
    commandId: str,
    displayName: str,
    description: str,
    deprecated: bool,
    lastUpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCustomMetricResponseTypeDef

```python
# UpdateCustomMetricResponseTypeDef definition

class UpdateCustomMetricResponseTypeDef(TypedDict):
    metricName: str,
    metricArn: str,
    metricType: CustomMetricTypeType,  # (1)
    displayName: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomMetricTypeType](./literals.md#custommetrictypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDimensionResponseTypeDef

```python
# UpdateDimensionResponseTypeDef definition

class UpdateDimensionResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    type: DimensionTypeType,  # (1)
    stringValues: List[str],
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainConfigurationResponseTypeDef

```python
# UpdateDomainConfigurationResponseTypeDef definition

class UpdateDomainConfigurationResponseTypeDef(TypedDict):
    domainConfigurationName: str,
    domainConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDynamicThingGroupResponseTypeDef

```python
# UpdateDynamicThingGroupResponseTypeDef definition

class UpdateDynamicThingGroupResponseTypeDef(TypedDict):
    version: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMitigationActionResponseTypeDef

```python
# UpdateMitigationActionResponseTypeDef definition

class UpdateMitigationActionResponseTypeDef(TypedDict):
    actionArn: str,
    actionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRoleAliasResponseTypeDef

```python
# UpdateRoleAliasResponseTypeDef definition

class UpdateRoleAliasResponseTypeDef(TypedDict):
    roleAlias: str,
    roleAliasArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScheduledAuditResponseTypeDef

```python
# UpdateScheduledAuditResponseTypeDef definition

class UpdateScheduledAuditResponseTypeDef(TypedDict):
    scheduledAuditArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStreamResponseTypeDef

```python
# UpdateStreamResponseTypeDef definition

class UpdateStreamResponseTypeDef(TypedDict):
    streamId: str,
    streamArn: str,
    description: str,
    streamVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThingGroupResponseTypeDef

```python
# UpdateThingGroupResponseTypeDef definition

class UpdateThingGroupResponseTypeDef(TypedDict):
    version: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThingGroupPropertiesOutputTypeDef

```python
# ThingGroupPropertiesOutputTypeDef definition

class ThingGroupPropertiesOutputTypeDef(TypedDict):
    thingGroupDescription: NotRequired[str],
    attributePayload: NotRequired[AttributePayloadOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AttributePayloadOutputTypeDef](./type_defs.md#attributepayloadoutputtypedef) 
## CreateThingRequestRequestTypeDef

```python
# CreateThingRequestRequestTypeDef definition

class CreateThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    thingTypeName: NotRequired[str],
    attributePayload: NotRequired[AttributePayloadTypeDef],  # (1)
    billingGroupName: NotRequired[str],
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) 
## UpdateThingRequestRequestTypeDef

```python
# UpdateThingRequestRequestTypeDef definition

class UpdateThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    thingTypeName: NotRequired[str],
    attributePayload: NotRequired[AttributePayloadTypeDef],  # (1)
    expectedVersion: NotRequired[int],
    removeThingType: NotRequired[bool],
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) 
## ListAuditMitigationActionsExecutionsResponseTypeDef

```python
# ListAuditMitigationActionsExecutionsResponseTypeDef definition

class ListAuditMitigationActionsExecutionsResponseTypeDef(TypedDict):
    actionsExecutions: List[AuditMitigationActionExecutionMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditMitigationActionExecutionMetadataTypeDef](./type_defs.md#auditmitigationactionexecutionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAuditMitigationActionsTasksResponseTypeDef

```python
# ListAuditMitigationActionsTasksResponseTypeDef definition

class ListAuditMitigationActionsTasksResponseTypeDef(TypedDict):
    tasks: List[AuditMitigationActionsTaskMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditMitigationActionsTaskMetadataTypeDef](./type_defs.md#auditmitigationactionstaskmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAuditMitigationActionsTaskRequestRequestTypeDef

```python
# StartAuditMitigationActionsTaskRequestRequestTypeDef definition

class StartAuditMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
    target: AuditMitigationActionsTaskTargetTypeDef,  # (1)
    auditCheckToActionsMapping: Mapping[str, Sequence[str]],
    clientRequestToken: str,
```

1. See [:material-code-braces: AuditMitigationActionsTaskTargetTypeDef](./type_defs.md#auditmitigationactionstasktargettypedef) 
## DescribeAccountAuditConfigurationResponseTypeDef

```python
# DescribeAccountAuditConfigurationResponseTypeDef definition

class DescribeAccountAuditConfigurationResponseTypeDef(TypedDict):
    roleArn: str,
    auditNotificationTargetConfigurations: Dict[AuditNotificationTypeType, AuditNotificationTargetTypeDef],  # (1)
    auditCheckConfigurations: Dict[str, AuditCheckConfigurationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuditNotificationTypeType](./literals.md#auditnotificationtypetype) [:material-code-braces: AuditNotificationTargetTypeDef](./type_defs.md#auditnotificationtargettypedef) 
2. See [:material-code-braces: AuditCheckConfigurationTypeDef](./type_defs.md#auditcheckconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountAuditConfigurationRequestRequestTypeDef

```python
# UpdateAccountAuditConfigurationRequestRequestTypeDef definition

class UpdateAccountAuditConfigurationRequestRequestTypeDef(TypedDict):
    roleArn: NotRequired[str],
    auditNotificationTargetConfigurations: NotRequired[Mapping[AuditNotificationTypeType, AuditNotificationTargetTypeDef]],  # (1)
    auditCheckConfigurations: NotRequired[Mapping[str, AuditCheckConfigurationTypeDef]],  # (2)
```

1. See [:material-code-brackets: AuditNotificationTypeType](./literals.md#auditnotificationtypetype) [:material-code-braces: AuditNotificationTargetTypeDef](./type_defs.md#auditnotificationtargettypedef) 
2. See [:material-code-braces: AuditCheckConfigurationTypeDef](./type_defs.md#auditcheckconfigurationtypedef) 
## ListAuditTasksResponseTypeDef

```python
# ListAuditTasksResponseTypeDef definition

class ListAuditTasksResponseTypeDef(TypedDict):
    tasks: List[AuditTaskMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditTaskMetadataTypeDef](./type_defs.md#audittaskmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAuthorizerResponseTypeDef

```python
# DescribeAuthorizerResponseTypeDef definition

class DescribeAuthorizerResponseTypeDef(TypedDict):
    authorizerDescription: AuthorizerDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizerDescriptionTypeDef](./type_defs.md#authorizerdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDefaultAuthorizerResponseTypeDef

```python
# DescribeDefaultAuthorizerResponseTypeDef definition

class DescribeDefaultAuthorizerResponseTypeDef(TypedDict):
    authorizerDescription: AuthorizerDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizerDescriptionTypeDef](./type_defs.md#authorizerdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAuthorizersResponseTypeDef

```python
# ListAuthorizersResponseTypeDef definition

class ListAuthorizersResponseTypeDef(TypedDict):
    authorizers: List[AuthorizerSummaryTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizerSummaryTypeDef](./type_defs.md#authorizersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AwsJobAbortConfigTypeDef

```python
# AwsJobAbortConfigTypeDef definition

class AwsJobAbortConfigTypeDef(TypedDict):
    abortCriteriaList: Sequence[AwsJobAbortCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: AwsJobAbortCriteriaTypeDef](./type_defs.md#awsjobabortcriteriatypedef) 
## AwsJobExponentialRolloutRateTypeDef

```python
# AwsJobExponentialRolloutRateTypeDef definition

class AwsJobExponentialRolloutRateTypeDef(TypedDict):
    baseRatePerMinute: int,
    incrementFactor: float,
    rateIncreaseCriteria: AwsJobRateIncreaseCriteriaTypeDef,  # (1)
```

1. See [:material-code-braces: AwsJobRateIncreaseCriteriaTypeDef](./type_defs.md#awsjobrateincreasecriteriatypedef) 
## BehaviorCriteriaOutputTypeDef

```python
# BehaviorCriteriaOutputTypeDef definition

class BehaviorCriteriaOutputTypeDef(TypedDict):
    comparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
    value: NotRequired[MetricValueOutputTypeDef],  # (2)
    durationSeconds: NotRequired[int],
    consecutiveDatapointsToAlarm: NotRequired[int],
    consecutiveDatapointsToClear: NotRequired[int],
    statisticalThreshold: NotRequired[StatisticalThresholdTypeDef],  # (3)
    mlDetectionConfig: NotRequired[MachineLearningDetectionConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 
3. See [:material-code-braces: StatisticalThresholdTypeDef](./type_defs.md#statisticalthresholdtypedef) 
4. See [:material-code-braces: MachineLearningDetectionConfigTypeDef](./type_defs.md#machinelearningdetectionconfigtypedef) 
## GetBehaviorModelTrainingSummariesResponseTypeDef

```python
# GetBehaviorModelTrainingSummariesResponseTypeDef definition

class GetBehaviorModelTrainingSummariesResponseTypeDef(TypedDict):
    summaries: List[BehaviorModelTrainingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BehaviorModelTrainingSummaryTypeDef](./type_defs.md#behaviormodeltrainingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricToRetainTypeDef

```python
# MetricToRetainTypeDef definition

class MetricToRetainTypeDef(TypedDict):
    metric: str,
    metricDimension: NotRequired[MetricDimensionTypeDef],  # (1)
    exportMetric: NotRequired[bool],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## DescribeBillingGroupResponseTypeDef

```python
# DescribeBillingGroupResponseTypeDef definition

class DescribeBillingGroupResponseTypeDef(TypedDict):
    billingGroupName: str,
    billingGroupId: str,
    billingGroupArn: str,
    version: int,
    billingGroupProperties: BillingGroupPropertiesTypeDef,  # (1)
    billingGroupMetadata: BillingGroupMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillingGroupPropertiesTypeDef](./type_defs.md#billinggrouppropertiestypedef) 
2. See [:material-code-braces: BillingGroupMetadataTypeDef](./type_defs.md#billinggroupmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillingGroupRequestRequestTypeDef

```python
# UpdateBillingGroupRequestRequestTypeDef definition

class UpdateBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: str,
    billingGroupProperties: BillingGroupPropertiesTypeDef,  # (1)
    expectedVersion: NotRequired[int],
```

1. See [:material-code-braces: BillingGroupPropertiesTypeDef](./type_defs.md#billinggrouppropertiestypedef) 
## CodeSigningSignatureTypeDef

```python
# CodeSigningSignatureTypeDef definition

class CodeSigningSignatureTypeDef(TypedDict):
    inlineDocument: NotRequired[BlobTypeDef],
```

## CommandParameterValueTypeDef

```python
# CommandParameterValueTypeDef definition

class CommandParameterValueTypeDef(TypedDict):
    S: NotRequired[str],
    B: NotRequired[bool],
    I: NotRequired[int],
    L: NotRequired[int],
    D: NotRequired[float],
    BIN: NotRequired[BlobTypeDef],
    UL: NotRequired[str],
```

## CommandPayloadTypeDef

```python
# CommandPayloadTypeDef definition

class CommandPayloadTypeDef(TypedDict):
    content: NotRequired[BlobTypeDef],
    contentType: NotRequired[str],
```

## MqttContextTypeDef

```python
# MqttContextTypeDef definition

class MqttContextTypeDef(TypedDict):
    username: NotRequired[str],
    password: NotRequired[BlobTypeDef],
    clientId: NotRequired[str],
```

## GetBucketsAggregationResponseTypeDef

```python
# GetBucketsAggregationResponseTypeDef definition

class GetBucketsAggregationResponseTypeDef(TypedDict):
    totalCount: int,
    buckets: List[BucketTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BucketsAggregationTypeTypeDef

```python
# BucketsAggregationTypeTypeDef definition

class BucketsAggregationTypeTypeDef(TypedDict):
    termsAggregation: NotRequired[TermsAggregationTypeDef],  # (1)
```

1. See [:material-code-braces: TermsAggregationTypeDef](./type_defs.md#termsaggregationtypedef) 
## CACertificateDescriptionTypeDef

```python
# CACertificateDescriptionTypeDef definition

class CACertificateDescriptionTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateId: NotRequired[str],
    status: NotRequired[CACertificateStatusType],  # (1)
    certificatePem: NotRequired[str],
    ownedBy: NotRequired[str],
    creationDate: NotRequired[datetime],
    autoRegistrationStatus: NotRequired[AutoRegistrationStatusType],  # (2)
    lastModifiedDate: NotRequired[datetime],
    customerVersion: NotRequired[int],
    generationId: NotRequired[str],
    validity: NotRequired[CertificateValidityTypeDef],  # (3)
    certificateMode: NotRequired[CertificateModeType],  # (4)
```

1. See [:material-code-brackets: CACertificateStatusType](./literals.md#cacertificatestatustype) 
2. See [:material-code-brackets: AutoRegistrationStatusType](./literals.md#autoregistrationstatustype) 
3. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
4. See [:material-code-brackets: CertificateModeType](./literals.md#certificatemodetype) 
## ListCACertificatesResponseTypeDef

```python
# ListCACertificatesResponseTypeDef definition

class ListCACertificatesResponseTypeDef(TypedDict):
    certificates: List[CACertificateTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CACertificateTypeDef](./type_defs.md#cacertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CertificateDescriptionTypeDef

```python
# CertificateDescriptionTypeDef definition

class CertificateDescriptionTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateId: NotRequired[str],
    caCertificateId: NotRequired[str],
    status: NotRequired[CertificateStatusType],  # (1)
    certificatePem: NotRequired[str],
    ownedBy: NotRequired[str],
    previousOwnedBy: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
    customerVersion: NotRequired[int],
    transferData: NotRequired[TransferDataTypeDef],  # (2)
    generationId: NotRequired[str],
    validity: NotRequired[CertificateValidityTypeDef],  # (3)
    certificateMode: NotRequired[CertificateModeType],  # (4)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: TransferDataTypeDef](./type_defs.md#transferdatatypedef) 
3. See [:material-code-braces: CertificateValidityTypeDef](./type_defs.md#certificatevaliditytypedef) 
4. See [:material-code-brackets: CertificateModeType](./literals.md#certificatemodetype) 
## ListCertificateProvidersResponseTypeDef

```python
# ListCertificateProvidersResponseTypeDef definition

class ListCertificateProvidersResponseTypeDef(TypedDict):
    certificateProviders: List[CertificateProviderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CertificateProviderSummaryTypeDef](./type_defs.md#certificateprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCertificatesByCAResponseTypeDef

```python
# ListCertificatesByCAResponseTypeDef definition

class ListCertificatesByCAResponseTypeDef(TypedDict):
    certificates: List[CertificateTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCertificatesResponseTypeDef

```python
# ListCertificatesResponseTypeDef definition

class ListCertificatesResponseTypeDef(TypedDict):
    certificates: List[CertificateTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomCodeSigningOutputTypeDef

```python
# CustomCodeSigningOutputTypeDef definition

class CustomCodeSigningOutputTypeDef(TypedDict):
    signature: NotRequired[CodeSigningSignatureOutputTypeDef],  # (1)
    certificateChain: NotRequired[CodeSigningCertificateChainTypeDef],  # (2)
    hashAlgorithm: NotRequired[str],
    signatureAlgorithm: NotRequired[str],
```

1. See [:material-code-braces: CodeSigningSignatureOutputTypeDef](./type_defs.md#codesigningsignatureoutputtypedef) 
2. See [:material-code-braces: CodeSigningCertificateChainTypeDef](./type_defs.md#codesigningcertificatechaintypedef) 
## ListCommandExecutionsResponseTypeDef

```python
# ListCommandExecutionsResponseTypeDef definition

class ListCommandExecutionsResponseTypeDef(TypedDict):
    commandExecutions: List[CommandExecutionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommandExecutionSummaryTypeDef](./type_defs.md#commandexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommandParameterOutputTypeDef

```python
# CommandParameterOutputTypeDef definition

class CommandParameterOutputTypeDef(TypedDict):
    name: str,
    value: NotRequired[CommandParameterValueOutputTypeDef],  # (1)
    defaultValue: NotRequired[CommandParameterValueOutputTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 
2. See [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 
## ListCommandsResponseTypeDef

```python
# ListCommandsResponseTypeDef definition

class ListCommandsResponseTypeDef(TypedDict):
    commands: List[CommandSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommandSummaryTypeDef](./type_defs.md#commandsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventConfigurationsResponseTypeDef

```python
# DescribeEventConfigurationsResponseTypeDef definition

class DescribeEventConfigurationsResponseTypeDef(TypedDict):
    eventConfigurations: Dict[EventTypeType, ConfigurationTypeDef],  # (1)
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventConfigurationsRequestRequestTypeDef

```python
# UpdateEventConfigurationsRequestRequestTypeDef definition

class UpdateEventConfigurationsRequestRequestTypeDef(TypedDict):
    eventConfigurations: NotRequired[Mapping[EventTypeType, ConfigurationTypeDef]],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
## ListAuditMitigationActionsTasksRequestRequestTypeDef

```python
# ListAuditMitigationActionsTasksRequestRequestTypeDef definition

class ListAuditMitigationActionsTasksRequestRequestTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    auditTaskId: NotRequired[str],
    findingId: NotRequired[str],
    taskStatus: NotRequired[AuditMitigationActionsTaskStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
## ListAuditTasksRequestRequestTypeDef

```python
# ListAuditTasksRequestRequestTypeDef definition

class ListAuditTasksRequestRequestTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    taskType: NotRequired[AuditTaskTypeType],  # (1)
    taskStatus: NotRequired[AuditTaskStatusType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
2. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
## ListDetectMitigationActionsExecutionsRequestRequestTypeDef

```python
# ListDetectMitigationActionsExecutionsRequestRequestTypeDef definition

class ListDetectMitigationActionsExecutionsRequestRequestTypeDef(TypedDict):
    taskId: NotRequired[str],
    violationId: NotRequired[str],
    thingName: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDetectMitigationActionsTasksRequestRequestTypeDef

```python
# ListDetectMitigationActionsTasksRequestRequestTypeDef definition

class ListDetectMitigationActionsTasksRequestRequestTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMetricValuesRequestRequestTypeDef

```python
# ListMetricValuesRequestRequestTypeDef definition

class ListMetricValuesRequestRequestTypeDef(TypedDict):
    thingName: str,
    metricName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    dimensionName: NotRequired[str],
    dimensionValueOperator: NotRequired[DimensionValueOperatorType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype) 
## ListViolationEventsRequestRequestTypeDef

```python
# ListViolationEventsRequestRequestTypeDef definition

class ListViolationEventsRequestRequestTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behaviorCriteriaType: NotRequired[BehaviorCriteriaTypeType],  # (1)
    listSuppressedAlerts: NotRequired[bool],
    verificationState: NotRequired[VerificationStateType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
## ViolationEventOccurrenceRangeTypeDef

```python
# ViolationEventOccurrenceRangeTypeDef definition

class ViolationEventOccurrenceRangeTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

## CreateAuthorizerRequestRequestTypeDef

```python
# CreateAuthorizerRequestRequestTypeDef definition

class CreateAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
    authorizerFunctionArn: str,
    tokenKeyName: NotRequired[str],
    tokenSigningPublicKeys: NotRequired[Mapping[str, str]],
    status: NotRequired[AuthorizerStatusType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    signingDisabled: NotRequired[bool],
    enableCachingForHttp: NotRequired[bool],
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBillingGroupRequestRequestTypeDef

```python
# CreateBillingGroupRequestRequestTypeDef definition

class CreateBillingGroupRequestRequestTypeDef(TypedDict):
    billingGroupName: str,
    billingGroupProperties: NotRequired[BillingGroupPropertiesTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: BillingGroupPropertiesTypeDef](./type_defs.md#billinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCertificateProviderRequestRequestTypeDef

```python
# CreateCertificateProviderRequestRequestTypeDef definition

class CreateCertificateProviderRequestRequestTypeDef(TypedDict):
    certificateProviderName: str,
    lambdaFunctionArn: str,
    accountDefaultForOperations: Sequence[CertificateProviderOperationType],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: CertificateProviderOperationType](./literals.md#certificateprovideroperationtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCustomMetricRequestRequestTypeDef

```python
# CreateCustomMetricRequestRequestTypeDef definition

class CreateCustomMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
    metricType: CustomMetricTypeType,  # (1)
    clientRequestToken: str,
    displayName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: CustomMetricTypeType](./literals.md#custommetrictypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDimensionRequestRequestTypeDef

```python
# CreateDimensionRequestRequestTypeDef definition

class CreateDimensionRequestRequestTypeDef(TypedDict):
    name: str,
    type: DimensionTypeType,  # (1)
    stringValues: Sequence[str],
    clientRequestToken: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFleetMetricRequestRequestTypeDef

```python
# CreateFleetMetricRequestRequestTypeDef definition

class CreateFleetMetricRequestRequestTypeDef(TypedDict):
    metricName: str,
    queryString: str,
    aggregationType: AggregationTypeTypeDef,  # (1)
    period: int,
    aggregationField: str,
    description: NotRequired[str],
    queryVersion: NotRequired[str],
    indexName: NotRequired[str],
    unit: NotRequired[FleetMetricUnitType],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: AggregationTypeTypeDef](./type_defs.md#aggregationtypetypedef) 
2. See [:material-code-brackets: FleetMetricUnitType](./literals.md#fleetmetricunittype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePolicyRequestRequestTypeDef

```python
# CreatePolicyRequestRequestTypeDef definition

class CreatePolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyDocument: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRoleAliasRequestRequestTypeDef

```python
# CreateRoleAliasRequestRequestTypeDef definition

class CreateRoleAliasRequestRequestTypeDef(TypedDict):
    roleAlias: str,
    roleArn: str,
    credentialDurationSeconds: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateScheduledAuditRequestRequestTypeDef

```python
# CreateScheduledAuditRequestRequestTypeDef definition

class CreateScheduledAuditRequestRequestTypeDef(TypedDict):
    frequency: AuditFrequencyType,  # (1)
    targetCheckNames: Sequence[str],
    scheduledAuditName: str,
    dayOfMonth: NotRequired[str],
    dayOfWeek: NotRequired[DayOfWeekType],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDomainConfigurationRequestRequestTypeDef

```python
# CreateDomainConfigurationRequestRequestTypeDef definition

class CreateDomainConfigurationRequestRequestTypeDef(TypedDict):
    domainConfigurationName: str,
    domainName: NotRequired[str],
    serverCertificateArns: NotRequired[Sequence[str]],
    validationCertificateArn: NotRequired[str],
    authorizerConfig: NotRequired[AuthorizerConfigTypeDef],  # (1)
    serviceType: NotRequired[ServiceTypeType],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    tlsConfig: NotRequired[TlsConfigTypeDef],  # (4)
    serverCertificateConfig: NotRequired[ServerCertificateConfigTypeDef],  # (5)
    authenticationType: NotRequired[AuthenticationTypeType],  # (6)
    applicationProtocol: NotRequired[ApplicationProtocolType],  # (7)
    clientCertificateConfig: NotRequired[ClientCertificateConfigTypeDef],  # (8)
```

1. See [:material-code-braces: AuthorizerConfigTypeDef](./type_defs.md#authorizerconfigtypedef) 
2. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
5. See [:material-code-braces: ServerCertificateConfigTypeDef](./type_defs.md#servercertificateconfigtypedef) 
6. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
7. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
8. See [:material-code-braces: ClientCertificateConfigTypeDef](./type_defs.md#clientcertificateconfigtypedef) 
## UpdateDomainConfigurationRequestRequestTypeDef

```python
# UpdateDomainConfigurationRequestRequestTypeDef definition

class UpdateDomainConfigurationRequestRequestTypeDef(TypedDict):
    domainConfigurationName: str,
    authorizerConfig: NotRequired[AuthorizerConfigTypeDef],  # (1)
    domainConfigurationStatus: NotRequired[DomainConfigurationStatusType],  # (2)
    removeAuthorizerConfig: NotRequired[bool],
    tlsConfig: NotRequired[TlsConfigTypeDef],  # (3)
    serverCertificateConfig: NotRequired[ServerCertificateConfigTypeDef],  # (4)
    authenticationType: NotRequired[AuthenticationTypeType],  # (5)
    applicationProtocol: NotRequired[ApplicationProtocolType],  # (6)
    clientCertificateConfig: NotRequired[ClientCertificateConfigTypeDef],  # (7)
```

1. See [:material-code-braces: AuthorizerConfigTypeDef](./type_defs.md#authorizerconfigtypedef) 
2. See [:material-code-brackets: DomainConfigurationStatusType](./literals.md#domainconfigurationstatustype) 
3. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
4. See [:material-code-braces: ServerCertificateConfigTypeDef](./type_defs.md#servercertificateconfigtypedef) 
5. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
6. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
7. See [:material-code-braces: ClientCertificateConfigTypeDef](./type_defs.md#clientcertificateconfigtypedef) 
## SchedulingConfigOutputTypeDef

```python
# SchedulingConfigOutputTypeDef definition

class SchedulingConfigOutputTypeDef(TypedDict):
    startTime: NotRequired[str],
    endTime: NotRequired[str],
    endBehavior: NotRequired[JobEndBehaviorType],  # (1)
    maintenanceWindows: NotRequired[List[MaintenanceWindowTypeDef]],  # (2)
```

1. See [:material-code-brackets: JobEndBehaviorType](./literals.md#jobendbehaviortype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
## SchedulingConfigTypeDef

```python
# SchedulingConfigTypeDef definition

class SchedulingConfigTypeDef(TypedDict):
    startTime: NotRequired[str],
    endTime: NotRequired[str],
    endBehavior: NotRequired[JobEndBehaviorType],  # (1)
    maintenanceWindows: NotRequired[Sequence[MaintenanceWindowTypeDef]],  # (2)
```

1. See [:material-code-brackets: JobEndBehaviorType](./literals.md#jobendbehaviortype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
## CreateKeysAndCertificateResponseTypeDef

```python
# CreateKeysAndCertificateResponseTypeDef definition

class CreateKeysAndCertificateResponseTypeDef(TypedDict):
    certificateArn: str,
    certificateId: str,
    certificatePem: str,
    keyPair: KeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPairTypeDef](./type_defs.md#keypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisioningClaimResponseTypeDef

```python
# CreateProvisioningClaimResponseTypeDef definition

class CreateProvisioningClaimResponseTypeDef(TypedDict):
    certificateId: str,
    certificatePem: str,
    keyPair: KeyPairTypeDef,  # (1)
    expiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPairTypeDef](./type_defs.md#keypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisioningTemplateRequestRequestTypeDef

```python
# CreateProvisioningTemplateRequestRequestTypeDef definition

class CreateProvisioningTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
    templateBody: str,
    provisioningRoleArn: str,
    description: NotRequired[str],
    enabled: NotRequired[bool],
    preProvisioningHook: NotRequired[ProvisioningHookTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    type: NotRequired[TemplateTypeType],  # (3)
```

1. See [:material-code-braces: ProvisioningHookTypeDef](./type_defs.md#provisioninghooktypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## DescribeProvisioningTemplateResponseTypeDef

```python
# DescribeProvisioningTemplateResponseTypeDef definition

class DescribeProvisioningTemplateResponseTypeDef(TypedDict):
    templateArn: str,
    templateName: str,
    description: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    defaultVersionId: int,
    templateBody: str,
    enabled: bool,
    provisioningRoleArn: str,
    preProvisioningHook: ProvisioningHookTypeDef,  # (1)
    type: TemplateTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProvisioningHookTypeDef](./type_defs.md#provisioninghooktypedef) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProvisioningTemplateRequestRequestTypeDef

```python
# UpdateProvisioningTemplateRequestRequestTypeDef definition

class UpdateProvisioningTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
    description: NotRequired[str],
    enabled: NotRequired[bool],
    defaultVersionId: NotRequired[int],
    provisioningRoleArn: NotRequired[str],
    preProvisioningHook: NotRequired[ProvisioningHookTypeDef],  # (1)
    removePreProvisioningHook: NotRequired[bool],
```

1. See [:material-code-braces: ProvisioningHookTypeDef](./type_defs.md#provisioninghooktypedef) 
## DescribeAuditTaskResponseTypeDef

```python
# DescribeAuditTaskResponseTypeDef definition

class DescribeAuditTaskResponseTypeDef(TypedDict):
    taskStatus: AuditTaskStatusType,  # (1)
    taskType: AuditTaskTypeType,  # (2)
    taskStartTime: datetime,
    taskStatistics: TaskStatisticsTypeDef,  # (3)
    scheduledAuditName: str,
    auditDetails: Dict[str, AuditCheckDetailsTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
2. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
3. See [:material-code-braces: TaskStatisticsTypeDef](./type_defs.md#taskstatisticstypedef) 
4. See [:material-code-braces: AuditCheckDetailsTypeDef](./type_defs.md#auditcheckdetailstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterCACertificateRequestRequestTypeDef

```python
# RegisterCACertificateRequestRequestTypeDef definition

class RegisterCACertificateRequestRequestTypeDef(TypedDict):
    caCertificate: str,
    verificationCertificate: NotRequired[str],
    setAsActive: NotRequired[bool],
    allowAutoRegistration: NotRequired[bool],
    registrationConfig: NotRequired[RegistrationConfigTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    certificateMode: NotRequired[CertificateModeType],  # (3)
```

1. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: CertificateModeType](./literals.md#certificatemodetype) 
## UpdateCACertificateRequestRequestTypeDef

```python
# UpdateCACertificateRequestRequestTypeDef definition

class UpdateCACertificateRequestRequestTypeDef(TypedDict):
    certificateId: str,
    newStatus: NotRequired[CACertificateStatusType],  # (1)
    newAutoRegistrationStatus: NotRequired[AutoRegistrationStatusType],  # (2)
    registrationConfig: NotRequired[RegistrationConfigTypeDef],  # (3)
    removeAutoRegistration: NotRequired[bool],
```

1. See [:material-code-brackets: CACertificateStatusType](./literals.md#cacertificatestatustype) 
2. See [:material-code-brackets: AutoRegistrationStatusType](./literals.md#autoregistrationstatustype) 
3. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
## DescribeDomainConfigurationResponseTypeDef

```python
# DescribeDomainConfigurationResponseTypeDef definition

class DescribeDomainConfigurationResponseTypeDef(TypedDict):
    domainConfigurationName: str,
    domainConfigurationArn: str,
    domainName: str,
    serverCertificates: List[ServerCertificateSummaryTypeDef],  # (1)
    authorizerConfig: AuthorizerConfigTypeDef,  # (2)
    domainConfigurationStatus: DomainConfigurationStatusType,  # (3)
    serviceType: ServiceTypeType,  # (4)
    domainType: DomainTypeType,  # (5)
    lastStatusChangeDate: datetime,
    tlsConfig: TlsConfigTypeDef,  # (6)
    serverCertificateConfig: ServerCertificateConfigTypeDef,  # (7)
    authenticationType: AuthenticationTypeType,  # (8)
    applicationProtocol: ApplicationProtocolType,  # (9)
    clientCertificateConfig: ClientCertificateConfigTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: ServerCertificateSummaryTypeDef](./type_defs.md#servercertificatesummarytypedef) 
2. See [:material-code-braces: AuthorizerConfigTypeDef](./type_defs.md#authorizerconfigtypedef) 
3. See [:material-code-brackets: DomainConfigurationStatusType](./literals.md#domainconfigurationstatustype) 
4. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
5. See [:material-code-brackets: DomainTypeType](./literals.md#domaintypetype) 
6. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
7. See [:material-code-braces: ServerCertificateConfigTypeDef](./type_defs.md#servercertificateconfigtypedef) 
8. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
9. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
10. See [:material-code-braces: ClientCertificateConfigTypeDef](./type_defs.md#clientcertificateconfigtypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeManagedJobTemplateResponseTypeDef

```python
# DescribeManagedJobTemplateResponseTypeDef definition

class DescribeManagedJobTemplateResponseTypeDef(TypedDict):
    templateName: str,
    templateArn: str,
    description: str,
    templateVersion: str,
    environments: List[str],
    documentParameters: List[DocumentParameterTypeDef],  # (1)
    document: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentParameterTypeDef](./type_defs.md#documentparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRoleAliasResponseTypeDef

```python
# DescribeRoleAliasResponseTypeDef definition

class DescribeRoleAliasResponseTypeDef(TypedDict):
    roleAliasDescription: RoleAliasDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleAliasDescriptionTypeDef](./type_defs.md#rolealiasdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    s3Destination: NotRequired[S3DestinationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## ListDetectMitigationActionsExecutionsResponseTypeDef

```python
# ListDetectMitigationActionsExecutionsResponseTypeDef definition

class ListDetectMitigationActionsExecutionsResponseTypeDef(TypedDict):
    actionsExecutions: List[DetectMitigationActionExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DetectMitigationActionExecutionTypeDef](./type_defs.md#detectmitigationactionexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainConfigurationsResponseTypeDef

```python
# ListDomainConfigurationsResponseTypeDef definition

class ListDomainConfigurationsResponseTypeDef(TypedDict):
    domainConfigurations: List[DomainConfigurationSummaryTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainConfigurationSummaryTypeDef](./type_defs.md#domainconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DynamoDBv2ActionTypeDef

```python
# DynamoDBv2ActionTypeDef definition

class DynamoDBv2ActionTypeDef(TypedDict):
    roleArn: str,
    putItem: PutItemInputTypeDef,  # (1)
```

1. See [:material-code-braces: PutItemInputTypeDef](./type_defs.md#putiteminputtypedef) 
## GetEffectivePoliciesResponseTypeDef

```python
# GetEffectivePoliciesResponseTypeDef definition

class GetEffectivePoliciesResponseTypeDef(TypedDict):
    effectivePolicies: List[EffectivePolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EffectivePolicyTypeDef](./type_defs.md#effectivepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExponentialRolloutRateTypeDef

```python
# ExponentialRolloutRateTypeDef definition

class ExponentialRolloutRateTypeDef(TypedDict):
    baseRatePerMinute: int,
    incrementFactor: float,
    rateIncreaseCriteria: RateIncreaseCriteriaTypeDef,  # (1)
```

1. See [:material-code-braces: RateIncreaseCriteriaTypeDef](./type_defs.md#rateincreasecriteriatypedef) 
## ThingGroupIndexingConfigurationOutputTypeDef

```python
# ThingGroupIndexingConfigurationOutputTypeDef definition

class ThingGroupIndexingConfigurationOutputTypeDef(TypedDict):
    thingGroupIndexingMode: ThingGroupIndexingModeType,  # (1)
    managedFields: NotRequired[List[FieldTypeDef]],  # (2)
    customFields: NotRequired[List[FieldTypeDef]],  # (2)
```

1. See [:material-code-brackets: ThingGroupIndexingModeType](./literals.md#thinggroupindexingmodetype) 
2. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
3. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## ThingGroupIndexingConfigurationTypeDef

```python
# ThingGroupIndexingConfigurationTypeDef definition

class ThingGroupIndexingConfigurationTypeDef(TypedDict):
    thingGroupIndexingMode: ThingGroupIndexingModeType,  # (1)
    managedFields: NotRequired[Sequence[FieldTypeDef]],  # (2)
    customFields: NotRequired[Sequence[FieldTypeDef]],  # (2)
```

1. See [:material-code-brackets: ThingGroupIndexingModeType](./literals.md#thinggroupindexingmodetype) 
2. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
3. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## PackageVersionArtifactTypeDef

```python
# PackageVersionArtifactTypeDef definition

class PackageVersionArtifactTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## SbomTypeDef

```python
# SbomTypeDef definition

class SbomTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## StreamFileTypeDef

```python
# StreamFileTypeDef definition

class StreamFileTypeDef(TypedDict):
    fileId: NotRequired[int],
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## FileLocationTypeDef

```python
# FileLocationTypeDef definition

class FileLocationTypeDef(TypedDict):
    stream: NotRequired[StreamTypeDef],  # (1)
    s3Location: NotRequired[S3LocationTypeDef],  # (2)
```

1. See [:material-code-braces: StreamTypeDef](./type_defs.md#streamtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ListFleetMetricsResponseTypeDef

```python
# ListFleetMetricsResponseTypeDef definition

class ListFleetMetricsResponseTypeDef(TypedDict):
    fleetMetrics: List[FleetMetricNameAndArnTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetMetricNameAndArnTypeDef](./type_defs.md#fleetmetricnameandarntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndexingFilterOutputTypeDef

```python
# IndexingFilterOutputTypeDef definition

class IndexingFilterOutputTypeDef(TypedDict):
    namedShadowNames: NotRequired[List[str]],
    geoLocations: NotRequired[List[GeoLocationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: GeoLocationTargetTypeDef](./type_defs.md#geolocationtargettypedef) 
## IndexingFilterTypeDef

```python
# IndexingFilterTypeDef definition

class IndexingFilterTypeDef(TypedDict):
    namedShadowNames: NotRequired[Sequence[str]],
    geoLocations: NotRequired[Sequence[GeoLocationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: GeoLocationTargetTypeDef](./type_defs.md#geolocationtargettypedef) 
## GetBehaviorModelTrainingSummariesRequestPaginateTypeDef

```python
# GetBehaviorModelTrainingSummariesRequestPaginateTypeDef definition

class GetBehaviorModelTrainingSummariesRequestPaginateTypeDef(TypedDict):
    securityProfileName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListActiveViolationsRequestPaginateTypeDef

```python
# ListActiveViolationsRequestPaginateTypeDef definition

class ListActiveViolationsRequestPaginateTypeDef(TypedDict):
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behaviorCriteriaType: NotRequired[BehaviorCriteriaTypeType],  # (1)
    listSuppressedAlerts: NotRequired[bool],
    verificationState: NotRequired[VerificationStateType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedPoliciesRequestPaginateTypeDef

```python
# ListAttachedPoliciesRequestPaginateTypeDef definition

class ListAttachedPoliciesRequestPaginateTypeDef(TypedDict):
    target: str,
    recursive: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuditMitigationActionsExecutionsRequestPaginateTypeDef

```python
# ListAuditMitigationActionsExecutionsRequestPaginateTypeDef definition

class ListAuditMitigationActionsExecutionsRequestPaginateTypeDef(TypedDict):
    taskId: str,
    findingId: str,
    actionStatus: NotRequired[AuditMitigationActionsExecutionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuditMitigationActionsTasksRequestPaginateTypeDef

```python
# ListAuditMitigationActionsTasksRequestPaginateTypeDef definition

class ListAuditMitigationActionsTasksRequestPaginateTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    auditTaskId: NotRequired[str],
    findingId: NotRequired[str],
    taskStatus: NotRequired[AuditMitigationActionsTaskStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuditTasksRequestPaginateTypeDef

```python
# ListAuditTasksRequestPaginateTypeDef definition

class ListAuditTasksRequestPaginateTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    taskType: NotRequired[AuditTaskTypeType],  # (1)
    taskStatus: NotRequired[AuditTaskStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
2. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuthorizersRequestPaginateTypeDef

```python
# ListAuthorizersRequestPaginateTypeDef definition

class ListAuthorizersRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    status: NotRequired[AuthorizerStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingGroupsRequestPaginateTypeDef

```python
# ListBillingGroupsRequestPaginateTypeDef definition

class ListBillingGroupsRequestPaginateTypeDef(TypedDict):
    namePrefixFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCACertificatesRequestPaginateTypeDef

```python
# ListCACertificatesRequestPaginateTypeDef definition

class ListCACertificatesRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    templateName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCertificatesByCARequestPaginateTypeDef

```python
# ListCertificatesByCARequestPaginateTypeDef definition

class ListCertificatesByCARequestPaginateTypeDef(TypedDict):
    caCertificateId: str,
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCertificatesRequestPaginateTypeDef

```python
# ListCertificatesRequestPaginateTypeDef definition

class ListCertificatesRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandsRequestPaginateTypeDef

```python
# ListCommandsRequestPaginateTypeDef definition

class ListCommandsRequestPaginateTypeDef(TypedDict):
    namespace: NotRequired[CommandNamespaceType],  # (1)
    commandParameterName: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomMetricsRequestPaginateTypeDef

```python
# ListCustomMetricsRequestPaginateTypeDef definition

class ListCustomMetricsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDetectMitigationActionsExecutionsRequestPaginateTypeDef

```python
# ListDetectMitigationActionsExecutionsRequestPaginateTypeDef definition

class ListDetectMitigationActionsExecutionsRequestPaginateTypeDef(TypedDict):
    taskId: NotRequired[str],
    violationId: NotRequired[str],
    thingName: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDetectMitigationActionsTasksRequestPaginateTypeDef

```python
# ListDetectMitigationActionsTasksRequestPaginateTypeDef definition

class ListDetectMitigationActionsTasksRequestPaginateTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDimensionsRequestPaginateTypeDef

```python
# ListDimensionsRequestPaginateTypeDef definition

class ListDimensionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainConfigurationsRequestPaginateTypeDef

```python
# ListDomainConfigurationsRequestPaginateTypeDef definition

class ListDomainConfigurationsRequestPaginateTypeDef(TypedDict):
    serviceType: NotRequired[ServiceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetMetricsRequestPaginateTypeDef

```python
# ListFleetMetricsRequestPaginateTypeDef definition

class ListFleetMetricsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndicesRequestPaginateTypeDef

```python
# ListIndicesRequestPaginateTypeDef definition

class ListIndicesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobExecutionsForJobRequestPaginateTypeDef

```python
# ListJobExecutionsForJobRequestPaginateTypeDef definition

class ListJobExecutionsForJobRequestPaginateTypeDef(TypedDict):
    jobId: str,
    status: NotRequired[JobExecutionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobExecutionsForThingRequestPaginateTypeDef

```python
# ListJobExecutionsForThingRequestPaginateTypeDef definition

class ListJobExecutionsForThingRequestPaginateTypeDef(TypedDict):
    thingName: str,
    status: NotRequired[JobExecutionStatusType],  # (1)
    namespaceId: NotRequired[str],
    jobId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobTemplatesRequestPaginateTypeDef

```python
# ListJobTemplatesRequestPaginateTypeDef definition

class ListJobTemplatesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    status: NotRequired[JobStatusType],  # (1)
    targetSelection: NotRequired[TargetSelectionType],  # (2)
    thingGroupName: NotRequired[str],
    thingGroupId: NotRequired[str],
    namespaceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedJobTemplatesRequestPaginateTypeDef

```python
# ListManagedJobTemplatesRequestPaginateTypeDef definition

class ListManagedJobTemplatesRequestPaginateTypeDef(TypedDict):
    templateName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMetricValuesRequestPaginateTypeDef

```python
# ListMetricValuesRequestPaginateTypeDef definition

class ListMetricValuesRequestPaginateTypeDef(TypedDict):
    thingName: str,
    metricName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    dimensionName: NotRequired[str],
    dimensionValueOperator: NotRequired[DimensionValueOperatorType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMitigationActionsRequestPaginateTypeDef

```python
# ListMitigationActionsRequestPaginateTypeDef definition

class ListMitigationActionsRequestPaginateTypeDef(TypedDict):
    actionType: NotRequired[MitigationActionTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOTAUpdatesRequestPaginateTypeDef

```python
# ListOTAUpdatesRequestPaginateTypeDef definition

class ListOTAUpdatesRequestPaginateTypeDef(TypedDict):
    otaUpdateStatus: NotRequired[OTAUpdateStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutgoingCertificatesRequestPaginateTypeDef

```python
# ListOutgoingCertificatesRequestPaginateTypeDef definition

class ListOutgoingCertificatesRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackageVersionsRequestPaginateTypeDef

```python
# ListPackageVersionsRequestPaginateTypeDef definition

class ListPackageVersionsRequestPaginateTypeDef(TypedDict):
    packageName: str,
    status: NotRequired[PackageVersionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackagesRequestPaginateTypeDef

```python
# ListPackagesRequestPaginateTypeDef definition

class ListPackagesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesRequestPaginateTypeDef

```python
# ListPoliciesRequestPaginateTypeDef definition

class ListPoliciesRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyPrincipalsRequestPaginateTypeDef

```python
# ListPolicyPrincipalsRequestPaginateTypeDef definition

class ListPolicyPrincipalsRequestPaginateTypeDef(TypedDict):
    policyName: str,
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalPoliciesRequestPaginateTypeDef

```python
# ListPrincipalPoliciesRequestPaginateTypeDef definition

class ListPrincipalPoliciesRequestPaginateTypeDef(TypedDict):
    principal: str,
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalThingsRequestPaginateTypeDef

```python
# ListPrincipalThingsRequestPaginateTypeDef definition

class ListPrincipalThingsRequestPaginateTypeDef(TypedDict):
    principal: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalThingsV2RequestPaginateTypeDef

```python
# ListPrincipalThingsV2RequestPaginateTypeDef definition

class ListPrincipalThingsV2RequestPaginateTypeDef(TypedDict):
    principal: str,
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisioningTemplateVersionsRequestPaginateTypeDef

```python
# ListProvisioningTemplateVersionsRequestPaginateTypeDef definition

class ListProvisioningTemplateVersionsRequestPaginateTypeDef(TypedDict):
    templateName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisioningTemplatesRequestPaginateTypeDef

```python
# ListProvisioningTemplatesRequestPaginateTypeDef definition

class ListProvisioningTemplatesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRelatedResourcesForAuditFindingRequestPaginateTypeDef

```python
# ListRelatedResourcesForAuditFindingRequestPaginateTypeDef definition

class ListRelatedResourcesForAuditFindingRequestPaginateTypeDef(TypedDict):
    findingId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoleAliasesRequestPaginateTypeDef

```python
# ListRoleAliasesRequestPaginateTypeDef definition

class ListRoleAliasesRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSbomValidationResultsRequestPaginateTypeDef

```python
# ListSbomValidationResultsRequestPaginateTypeDef definition

class ListSbomValidationResultsRequestPaginateTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    validationResult: NotRequired[SbomValidationResultType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SbomValidationResultType](./literals.md#sbomvalidationresulttype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScheduledAuditsRequestPaginateTypeDef

```python
# ListScheduledAuditsRequestPaginateTypeDef definition

class ListScheduledAuditsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilesForTargetRequestPaginateTypeDef

```python
# ListSecurityProfilesForTargetRequestPaginateTypeDef definition

class ListSecurityProfilesForTargetRequestPaginateTypeDef(TypedDict):
    securityProfileTargetArn: str,
    recursive: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilesRequestPaginateTypeDef

```python
# ListSecurityProfilesRequestPaginateTypeDef definition

class ListSecurityProfilesRequestPaginateTypeDef(TypedDict):
    dimensionName: NotRequired[str],
    metricName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamsRequestPaginateTypeDef

```python
# ListStreamsRequestPaginateTypeDef definition

class ListStreamsRequestPaginateTypeDef(TypedDict):
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsForPolicyRequestPaginateTypeDef

```python
# ListTargetsForPolicyRequestPaginateTypeDef definition

class ListTargetsForPolicyRequestPaginateTypeDef(TypedDict):
    policyName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsForSecurityProfileRequestPaginateTypeDef

```python
# ListTargetsForSecurityProfileRequestPaginateTypeDef definition

class ListTargetsForSecurityProfileRequestPaginateTypeDef(TypedDict):
    securityProfileName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingGroupsForThingRequestPaginateTypeDef

```python
# ListThingGroupsForThingRequestPaginateTypeDef definition

class ListThingGroupsForThingRequestPaginateTypeDef(TypedDict):
    thingName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingGroupsRequestPaginateTypeDef

```python
# ListThingGroupsRequestPaginateTypeDef definition

class ListThingGroupsRequestPaginateTypeDef(TypedDict):
    parentGroup: NotRequired[str],
    namePrefixFilter: NotRequired[str],
    recursive: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingPrincipalsRequestPaginateTypeDef

```python
# ListThingPrincipalsRequestPaginateTypeDef definition

class ListThingPrincipalsRequestPaginateTypeDef(TypedDict):
    thingName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingPrincipalsV2RequestPaginateTypeDef

```python
# ListThingPrincipalsV2RequestPaginateTypeDef definition

class ListThingPrincipalsV2RequestPaginateTypeDef(TypedDict):
    thingName: str,
    thingPrincipalType: NotRequired[ThingPrincipalTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingRegistrationTaskReportsRequestPaginateTypeDef

```python
# ListThingRegistrationTaskReportsRequestPaginateTypeDef definition

class ListThingRegistrationTaskReportsRequestPaginateTypeDef(TypedDict):
    taskId: str,
    reportType: ReportTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingRegistrationTasksRequestPaginateTypeDef

```python
# ListThingRegistrationTasksRequestPaginateTypeDef definition

class ListThingRegistrationTasksRequestPaginateTypeDef(TypedDict):
    status: NotRequired[StatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingTypesRequestPaginateTypeDef

```python
# ListThingTypesRequestPaginateTypeDef definition

class ListThingTypesRequestPaginateTypeDef(TypedDict):
    thingTypeName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingsInBillingGroupRequestPaginateTypeDef

```python
# ListThingsInBillingGroupRequestPaginateTypeDef definition

class ListThingsInBillingGroupRequestPaginateTypeDef(TypedDict):
    billingGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingsInThingGroupRequestPaginateTypeDef

```python
# ListThingsInThingGroupRequestPaginateTypeDef definition

class ListThingsInThingGroupRequestPaginateTypeDef(TypedDict):
    thingGroupName: str,
    recursive: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThingsRequestPaginateTypeDef

```python
# ListThingsRequestPaginateTypeDef definition

class ListThingsRequestPaginateTypeDef(TypedDict):
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    thingTypeName: NotRequired[str],
    usePrefixAttributeValue: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTopicRuleDestinationsRequestPaginateTypeDef

```python
# ListTopicRuleDestinationsRequestPaginateTypeDef definition

class ListTopicRuleDestinationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTopicRulesRequestPaginateTypeDef

```python
# ListTopicRulesRequestPaginateTypeDef definition

class ListTopicRulesRequestPaginateTypeDef(TypedDict):
    topic: NotRequired[str],
    ruleDisabled: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListV2LoggingLevelsRequestPaginateTypeDef

```python
# ListV2LoggingLevelsRequestPaginateTypeDef definition

class ListV2LoggingLevelsRequestPaginateTypeDef(TypedDict):
    targetType: NotRequired[LogTargetTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViolationEventsRequestPaginateTypeDef

```python
# ListViolationEventsRequestPaginateTypeDef definition

class ListViolationEventsRequestPaginateTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behaviorCriteriaType: NotRequired[BehaviorCriteriaTypeType],  # (1)
    listSuppressedAlerts: NotRequired[bool],
    verificationState: NotRequired[VerificationStateType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCommandExecutionResponseTypeDef

```python
# GetCommandExecutionResponseTypeDef definition

class GetCommandExecutionResponseTypeDef(TypedDict):
    executionId: str,
    commandArn: str,
    targetArn: str,
    status: CommandExecutionStatusType,  # (1)
    statusReason: StatusReasonTypeDef,  # (2)
    result: Dict[str, CommandExecutionResultTypeDef],  # (3)
    parameters: Dict[str, CommandParameterValueOutputTypeDef],  # (4)
    executionTimeoutSeconds: int,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    startedAt: datetime,
    completedAt: datetime,
    timeToLive: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype) 
2. See [:material-code-braces: StatusReasonTypeDef](./type_defs.md#statusreasontypedef) 
3. See [:material-code-braces: CommandExecutionResultTypeDef](./type_defs.md#commandexecutionresulttypedef) 
4. See [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPackageConfigurationResponseTypeDef

```python
# GetPackageConfigurationResponseTypeDef definition

class GetPackageConfigurationResponseTypeDef(TypedDict):
    versionUpdateByJobsConfig: VersionUpdateByJobsConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionUpdateByJobsConfigTypeDef](./type_defs.md#versionupdatebyjobsconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageConfigurationRequestRequestTypeDef

```python
# UpdatePackageConfigurationRequestRequestTypeDef definition

class UpdatePackageConfigurationRequestRequestTypeDef(TypedDict):
    versionUpdateByJobsConfig: NotRequired[VersionUpdateByJobsConfigTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: VersionUpdateByJobsConfigTypeDef](./type_defs.md#versionupdatebyjobsconfigtypedef) 
## GetPercentilesResponseTypeDef

```python
# GetPercentilesResponseTypeDef definition

class GetPercentilesResponseTypeDef(TypedDict):
    percentiles: List[PercentPairTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PercentPairTypeDef](./type_defs.md#percentpairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStatisticsResponseTypeDef

```python
# GetStatisticsResponseTypeDef definition

class GetStatisticsResponseTypeDef(TypedDict):
    statistics: StatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatisticsTypeDef](./type_defs.md#statisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillingGroupsResponseTypeDef

```python
# ListBillingGroupsResponseTypeDef definition

class ListBillingGroupsResponseTypeDef(TypedDict):
    billingGroups: List[GroupNameAndArnTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupNameAndArnTypeDef](./type_defs.md#groupnameandarntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingGroupsForThingResponseTypeDef

```python
# ListThingGroupsForThingResponseTypeDef definition

class ListThingGroupsForThingResponseTypeDef(TypedDict):
    thingGroups: List[GroupNameAndArnTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupNameAndArnTypeDef](./type_defs.md#groupnameandarntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingGroupsResponseTypeDef

```python
# ListThingGroupsResponseTypeDef definition

class ListThingGroupsResponseTypeDef(TypedDict):
    thingGroups: List[GroupNameAndArnTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupNameAndArnTypeDef](./type_defs.md#groupnameandarntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThingGroupMetadataTypeDef

```python
# ThingGroupMetadataTypeDef definition

class ThingGroupMetadataTypeDef(TypedDict):
    parentGroupName: NotRequired[str],
    rootToParentThingGroups: NotRequired[List[GroupNameAndArnTypeDef]],  # (1)
    creationDate: NotRequired[datetime],
```

1. See [:material-code-braces: GroupNameAndArnTypeDef](./type_defs.md#groupnameandarntypedef) 
## HttpAuthorizationTypeDef

```python
# HttpAuthorizationTypeDef definition

class HttpAuthorizationTypeDef(TypedDict):
    sigv4: NotRequired[SigV4AuthorizationTypeDef],  # (1)
```

1. See [:material-code-braces: SigV4AuthorizationTypeDef](./type_defs.md#sigv4authorizationtypedef) 
## JobExecutionTypeDef

```python
# JobExecutionTypeDef definition

class JobExecutionTypeDef(TypedDict):
    jobId: NotRequired[str],
    status: NotRequired[JobExecutionStatusType],  # (1)
    forceCanceled: NotRequired[bool],
    statusDetails: NotRequired[JobExecutionStatusDetailsTypeDef],  # (2)
    thingArn: NotRequired[str],
    queuedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    executionNumber: NotRequired[int],
    versionNumber: NotRequired[int],
    approximateSecondsBeforeTimedOut: NotRequired[int],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: JobExecutionStatusDetailsTypeDef](./type_defs.md#jobexecutionstatusdetailstypedef) 
## JobExecutionSummaryForJobTypeDef

```python
# JobExecutionSummaryForJobTypeDef definition

class JobExecutionSummaryForJobTypeDef(TypedDict):
    thingArn: NotRequired[str],
    jobExecutionSummary: NotRequired[JobExecutionSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: JobExecutionSummaryTypeDef](./type_defs.md#jobexecutionsummarytypedef) 
## JobExecutionSummaryForThingTypeDef

```python
# JobExecutionSummaryForThingTypeDef definition

class JobExecutionSummaryForThingTypeDef(TypedDict):
    jobId: NotRequired[str],
    jobExecutionSummary: NotRequired[JobExecutionSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: JobExecutionSummaryTypeDef](./type_defs.md#jobexecutionsummarytypedef) 
## JobExecutionsRetryConfigOutputTypeDef

```python
# JobExecutionsRetryConfigOutputTypeDef definition

class JobExecutionsRetryConfigOutputTypeDef(TypedDict):
    criteriaList: List[RetryCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: RetryCriteriaTypeDef](./type_defs.md#retrycriteriatypedef) 
## JobExecutionsRetryConfigTypeDef

```python
# JobExecutionsRetryConfigTypeDef definition

class JobExecutionsRetryConfigTypeDef(TypedDict):
    criteriaList: Sequence[RetryCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: RetryCriteriaTypeDef](./type_defs.md#retrycriteriatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobTemplatesResponseTypeDef

```python
# ListJobTemplatesResponseTypeDef definition

class ListJobTemplatesResponseTypeDef(TypedDict):
    jobTemplates: List[JobTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTemplateSummaryTypeDef](./type_defs.md#jobtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KafkaActionOutputTypeDef

```python
# KafkaActionOutputTypeDef definition

class KafkaActionOutputTypeDef(TypedDict):
    destinationArn: str,
    topic: str,
    clientProperties: Dict[str, str],
    key: NotRequired[str],
    partition: NotRequired[str],
    headers: NotRequired[List[KafkaActionHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: KafkaActionHeaderTypeDef](./type_defs.md#kafkaactionheadertypedef) 
## KafkaActionTypeDef

```python
# KafkaActionTypeDef definition

class KafkaActionTypeDef(TypedDict):
    destinationArn: str,
    topic: str,
    clientProperties: Mapping[str, str],
    key: NotRequired[str],
    partition: NotRequired[str],
    headers: NotRequired[Sequence[KafkaActionHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: KafkaActionHeaderTypeDef](./type_defs.md#kafkaactionheadertypedef) 
## ListCommandExecutionsRequestPaginateTypeDef

```python
# ListCommandExecutionsRequestPaginateTypeDef definition

class ListCommandExecutionsRequestPaginateTypeDef(TypedDict):
    namespace: NotRequired[CommandNamespaceType],  # (1)
    status: NotRequired[CommandExecutionStatusType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    startedTimeFilter: NotRequired[TimeFilterTypeDef],  # (4)
    completedTimeFilter: NotRequired[TimeFilterTypeDef],  # (4)
    targetArn: NotRequired[str],
    commandArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
5. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandExecutionsRequestRequestTypeDef

```python
# ListCommandExecutionsRequestRequestTypeDef definition

class ListCommandExecutionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    namespace: NotRequired[CommandNamespaceType],  # (1)
    status: NotRequired[CommandExecutionStatusType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    startedTimeFilter: NotRequired[TimeFilterTypeDef],  # (4)
    completedTimeFilter: NotRequired[TimeFilterTypeDef],  # (4)
    targetArn: NotRequired[str],
    commandArn: NotRequired[str],
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
5. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
## ListManagedJobTemplatesResponseTypeDef

```python
# ListManagedJobTemplatesResponseTypeDef definition

class ListManagedJobTemplatesResponseTypeDef(TypedDict):
    managedJobTemplates: List[ManagedJobTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedJobTemplateSummaryTypeDef](./type_defs.md#managedjobtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMitigationActionsResponseTypeDef

```python
# ListMitigationActionsResponseTypeDef definition

class ListMitigationActionsResponseTypeDef(TypedDict):
    actionIdentifiers: List[MitigationActionIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MitigationActionIdentifierTypeDef](./type_defs.md#mitigationactionidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOTAUpdatesResponseTypeDef

```python
# ListOTAUpdatesResponseTypeDef definition

class ListOTAUpdatesResponseTypeDef(TypedDict):
    otaUpdates: List[OTAUpdateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OTAUpdateSummaryTypeDef](./type_defs.md#otaupdatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOutgoingCertificatesResponseTypeDef

```python
# ListOutgoingCertificatesResponseTypeDef definition

class ListOutgoingCertificatesResponseTypeDef(TypedDict):
    outgoingCertificates: List[OutgoingCertificateTypeDef],  # (1)
    nextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutgoingCertificateTypeDef](./type_defs.md#outgoingcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackageVersionsResponseTypeDef

```python
# ListPackageVersionsResponseTypeDef definition

class ListPackageVersionsResponseTypeDef(TypedDict):
    packageVersionSummaries: List[PackageVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageVersionSummaryTypeDef](./type_defs.md#packageversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackagesResponseTypeDef

```python
# ListPackagesResponseTypeDef definition

class ListPackagesResponseTypeDef(TypedDict):
    packageSummaries: List[PackageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageSummaryTypeDef](./type_defs.md#packagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyVersionsResponseTypeDef

```python
# ListPolicyVersionsResponseTypeDef definition

class ListPolicyVersionsResponseTypeDef(TypedDict):
    policyVersions: List[PolicyVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyVersionTypeDef](./type_defs.md#policyversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrincipalThingsV2ResponseTypeDef

```python
# ListPrincipalThingsV2ResponseTypeDef definition

class ListPrincipalThingsV2ResponseTypeDef(TypedDict):
    principalThingObjects: List[PrincipalThingObjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PrincipalThingObjectTypeDef](./type_defs.md#principalthingobjecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisioningTemplateVersionsResponseTypeDef

```python
# ListProvisioningTemplateVersionsResponseTypeDef definition

class ListProvisioningTemplateVersionsResponseTypeDef(TypedDict):
    versions: List[ProvisioningTemplateVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProvisioningTemplateVersionSummaryTypeDef](./type_defs.md#provisioningtemplateversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisioningTemplatesResponseTypeDef

```python
# ListProvisioningTemplatesResponseTypeDef definition

class ListProvisioningTemplatesResponseTypeDef(TypedDict):
    templates: List[ProvisioningTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProvisioningTemplateSummaryTypeDef](./type_defs.md#provisioningtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSbomValidationResultsResponseTypeDef

```python
# ListSbomValidationResultsResponseTypeDef definition

class ListSbomValidationResultsResponseTypeDef(TypedDict):
    validationResultSummaries: List[SbomValidationResultSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SbomValidationResultSummaryTypeDef](./type_defs.md#sbomvalidationresultsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScheduledAuditsResponseTypeDef

```python
# ListScheduledAuditsResponseTypeDef definition

class ListScheduledAuditsResponseTypeDef(TypedDict):
    scheduledAudits: List[ScheduledAuditMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduledAuditMetadataTypeDef](./type_defs.md#scheduledauditmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilesResponseTypeDef

```python
# ListSecurityProfilesResponseTypeDef definition

class ListSecurityProfilesResponseTypeDef(TypedDict):
    securityProfileIdentifiers: List[SecurityProfileIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityProfileIdentifierTypeDef](./type_defs.md#securityprofileidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamsResponseTypeDef

```python
# ListStreamsResponseTypeDef definition

class ListStreamsResponseTypeDef(TypedDict):
    streams: List[StreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSummaryTypeDef](./type_defs.md#streamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsForSecurityProfileResponseTypeDef

```python
# ListTargetsForSecurityProfileResponseTypeDef definition

class ListTargetsForSecurityProfileResponseTypeDef(TypedDict):
    securityProfileTargets: List[SecurityProfileTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityProfileTargetTypeDef](./type_defs.md#securityprofiletargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SecurityProfileTargetMappingTypeDef

```python
# SecurityProfileTargetMappingTypeDef definition

class SecurityProfileTargetMappingTypeDef(TypedDict):
    securityProfileIdentifier: NotRequired[SecurityProfileIdentifierTypeDef],  # (1)
    target: NotRequired[SecurityProfileTargetTypeDef],  # (2)
```

1. See [:material-code-braces: SecurityProfileIdentifierTypeDef](./type_defs.md#securityprofileidentifiertypedef) 
2. See [:material-code-braces: SecurityProfileTargetTypeDef](./type_defs.md#securityprofiletargettypedef) 
## ListThingPrincipalsV2ResponseTypeDef

```python
# ListThingPrincipalsV2ResponseTypeDef definition

class ListThingPrincipalsV2ResponseTypeDef(TypedDict):
    thingPrincipalObjects: List[ThingPrincipalObjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ThingPrincipalObjectTypeDef](./type_defs.md#thingprincipalobjecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingsResponseTypeDef

```python
# ListThingsResponseTypeDef definition

class ListThingsResponseTypeDef(TypedDict):
    things: List[ThingAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ThingAttributeTypeDef](./type_defs.md#thingattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTopicRulesResponseTypeDef

```python
# ListTopicRulesResponseTypeDef definition

class ListTopicRulesResponseTypeDef(TypedDict):
    rules: List[TopicRuleListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TopicRuleListItemTypeDef](./type_defs.md#topicrulelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LocationActionTypeDef

```python
# LocationActionTypeDef definition

class LocationActionTypeDef(TypedDict):
    roleArn: str,
    trackerName: str,
    deviceId: str,
    latitude: str,
    longitude: str,
    timestamp: NotRequired[LocationTimestampTypeDef],  # (1)
```

1. See [:material-code-braces: LocationTimestampTypeDef](./type_defs.md#locationtimestamptypedef) 
## LogTargetConfigurationTypeDef

```python
# LogTargetConfigurationTypeDef definition

class LogTargetConfigurationTypeDef(TypedDict):
    logTarget: NotRequired[LogTargetTypeDef],  # (1)
    logLevel: NotRequired[LogLevelType],  # (2)
```

1. See [:material-code-braces: LogTargetTypeDef](./type_defs.md#logtargettypedef) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## SetV2LoggingLevelRequestRequestTypeDef

```python
# SetV2LoggingLevelRequestRequestTypeDef definition

class SetV2LoggingLevelRequestRequestTypeDef(TypedDict):
    logTarget: LogTargetTypeDef,  # (1)
    logLevel: LogLevelType,  # (2)
```

1. See [:material-code-braces: LogTargetTypeDef](./type_defs.md#logtargettypedef) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## SetLoggingOptionsRequestRequestTypeDef

```python
# SetLoggingOptionsRequestRequestTypeDef definition

class SetLoggingOptionsRequestRequestTypeDef(TypedDict):
    loggingOptionsPayload: LoggingOptionsPayloadTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsPayloadTypeDef](./type_defs.md#loggingoptionspayloadtypedef) 
## MitigationActionParamsOutputTypeDef

```python
# MitigationActionParamsOutputTypeDef definition

class MitigationActionParamsOutputTypeDef(TypedDict):
    updateDeviceCertificateParams: NotRequired[UpdateDeviceCertificateParamsTypeDef],  # (1)
    updateCACertificateParams: NotRequired[UpdateCACertificateParamsTypeDef],  # (2)
    addThingsToThingGroupParams: NotRequired[AddThingsToThingGroupParamsOutputTypeDef],  # (3)
    replaceDefaultPolicyVersionParams: NotRequired[ReplaceDefaultPolicyVersionParamsTypeDef],  # (4)
    enableIoTLoggingParams: NotRequired[EnableIoTLoggingParamsTypeDef],  # (5)
    publishFindingToSnsParams: NotRequired[PublishFindingToSnsParamsTypeDef],  # (6)
```

1. See [:material-code-braces: UpdateDeviceCertificateParamsTypeDef](./type_defs.md#updatedevicecertificateparamstypedef) 
2. See [:material-code-braces: UpdateCACertificateParamsTypeDef](./type_defs.md#updatecacertificateparamstypedef) 
3. See [:material-code-braces: AddThingsToThingGroupParamsOutputTypeDef](./type_defs.md#addthingstothinggroupparamsoutputtypedef) 
4. See [:material-code-braces: ReplaceDefaultPolicyVersionParamsTypeDef](./type_defs.md#replacedefaultpolicyversionparamstypedef) 
5. See [:material-code-braces: EnableIoTLoggingParamsTypeDef](./type_defs.md#enableiotloggingparamstypedef) 
6. See [:material-code-braces: PublishFindingToSnsParamsTypeDef](./type_defs.md#publishfindingtosnsparamstypedef) 
## Mqtt5ConfigurationOutputTypeDef

```python
# Mqtt5ConfigurationOutputTypeDef definition

class Mqtt5ConfigurationOutputTypeDef(TypedDict):
    propagatingAttributes: NotRequired[List[PropagatingAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: PropagatingAttributeTypeDef](./type_defs.md#propagatingattributetypedef) 
## Mqtt5ConfigurationTypeDef

```python
# Mqtt5ConfigurationTypeDef definition

class Mqtt5ConfigurationTypeDef(TypedDict):
    propagatingAttributes: NotRequired[Sequence[PropagatingAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: PropagatingAttributeTypeDef](./type_defs.md#propagatingattributetypedef) 
## MqttHeadersOutputTypeDef

```python
# MqttHeadersOutputTypeDef definition

class MqttHeadersOutputTypeDef(TypedDict):
    payloadFormatIndicator: NotRequired[str],
    contentType: NotRequired[str],
    responseTopic: NotRequired[str],
    correlationData: NotRequired[str],
    messageExpiry: NotRequired[str],
    userProperties: NotRequired[List[UserPropertyTypeDef]],  # (1)
```

1. See [:material-code-braces: UserPropertyTypeDef](./type_defs.md#userpropertytypedef) 
## MqttHeadersTypeDef

```python
# MqttHeadersTypeDef definition

class MqttHeadersTypeDef(TypedDict):
    payloadFormatIndicator: NotRequired[str],
    contentType: NotRequired[str],
    responseTopic: NotRequired[str],
    correlationData: NotRequired[str],
    messageExpiry: NotRequired[str],
    userProperties: NotRequired[Sequence[UserPropertyTypeDef]],  # (1)
```

1. See [:material-code-braces: UserPropertyTypeDef](./type_defs.md#userpropertytypedef) 
## ResourceIdentifierTypeDef

```python
# ResourceIdentifierTypeDef definition

class ResourceIdentifierTypeDef(TypedDict):
    deviceCertificateId: NotRequired[str],
    caCertificateId: NotRequired[str],
    cognitoIdentityPoolId: NotRequired[str],
    clientId: NotRequired[str],
    policyVersionIdentifier: NotRequired[PolicyVersionIdentifierTypeDef],  # (1)
    account: NotRequired[str],
    iamRoleArn: NotRequired[str],
    roleAliasArn: NotRequired[str],
    issuerCertificateIdentifier: NotRequired[IssuerCertificateIdentifierTypeDef],  # (2)
    deviceCertificateArn: NotRequired[str],
```

1. See [:material-code-braces: PolicyVersionIdentifierTypeDef](./type_defs.md#policyversionidentifiertypedef) 
2. See [:material-code-braces: IssuerCertificateIdentifierTypeDef](./type_defs.md#issuercertificateidentifiertypedef) 
## ThingDocumentTypeDef

```python
# ThingDocumentTypeDef definition

class ThingDocumentTypeDef(TypedDict):
    thingName: NotRequired[str],
    thingId: NotRequired[str],
    thingTypeName: NotRequired[str],
    thingGroupNames: NotRequired[List[str]],
    attributes: NotRequired[Dict[str, str]],
    shadow: NotRequired[str],
    deviceDefender: NotRequired[str],
    connectivity: NotRequired[ThingConnectivityTypeDef],  # (1)
```

1. See [:material-code-braces: ThingConnectivityTypeDef](./type_defs.md#thingconnectivitytypedef) 
## TimestreamActionOutputTypeDef

```python
# TimestreamActionOutputTypeDef definition

class TimestreamActionOutputTypeDef(TypedDict):
    roleArn: str,
    databaseName: str,
    tableName: str,
    dimensions: List[TimestreamDimensionTypeDef],  # (1)
    timestamp: NotRequired[TimestreamTimestampTypeDef],  # (2)
```

1. See [:material-code-braces: TimestreamDimensionTypeDef](./type_defs.md#timestreamdimensiontypedef) 
2. See [:material-code-braces: TimestreamTimestampTypeDef](./type_defs.md#timestreamtimestamptypedef) 
## TimestreamActionTypeDef

```python
# TimestreamActionTypeDef definition

class TimestreamActionTypeDef(TypedDict):
    roleArn: str,
    databaseName: str,
    tableName: str,
    dimensions: Sequence[TimestreamDimensionTypeDef],  # (1)
    timestamp: NotRequired[TimestreamTimestampTypeDef],  # (2)
```

1. See [:material-code-braces: TimestreamDimensionTypeDef](./type_defs.md#timestreamdimensiontypedef) 
2. See [:material-code-braces: TimestreamTimestampTypeDef](./type_defs.md#timestreamtimestamptypedef) 
## TopicRuleDestinationConfigurationTypeDef

```python
# TopicRuleDestinationConfigurationTypeDef definition

class TopicRuleDestinationConfigurationTypeDef(TypedDict):
    httpUrlConfiguration: NotRequired[HttpUrlDestinationConfigurationTypeDef],  # (1)
    vpcConfiguration: NotRequired[VpcDestinationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: HttpUrlDestinationConfigurationTypeDef](./type_defs.md#httpurldestinationconfigurationtypedef) 
2. See [:material-code-braces: VpcDestinationConfigurationTypeDef](./type_defs.md#vpcdestinationconfigurationtypedef) 
## TopicRuleDestinationSummaryTypeDef

```python
# TopicRuleDestinationSummaryTypeDef definition

class TopicRuleDestinationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    status: NotRequired[TopicRuleDestinationStatusType],  # (1)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    statusReason: NotRequired[str],
    httpUrlSummary: NotRequired[HttpUrlDestinationSummaryTypeDef],  # (2)
    vpcDestinationSummary: NotRequired[VpcDestinationSummaryTypeDef],  # (3)
```

1. See [:material-code-brackets: TopicRuleDestinationStatusType](./literals.md#topicruledestinationstatustype) 
2. See [:material-code-braces: HttpUrlDestinationSummaryTypeDef](./type_defs.md#httpurldestinationsummarytypedef) 
3. See [:material-code-braces: VpcDestinationSummaryTypeDef](./type_defs.md#vpcdestinationsummarytypedef) 
## TopicRuleDestinationTypeDef

```python
# TopicRuleDestinationTypeDef definition

class TopicRuleDestinationTypeDef(TypedDict):
    arn: NotRequired[str],
    status: NotRequired[TopicRuleDestinationStatusType],  # (1)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    statusReason: NotRequired[str],
    httpUrlProperties: NotRequired[HttpUrlDestinationPropertiesTypeDef],  # (2)
    vpcProperties: NotRequired[VpcDestinationPropertiesTypeDef],  # (3)
```

1. See [:material-code-brackets: TopicRuleDestinationStatusType](./literals.md#topicruledestinationstatustype) 
2. See [:material-code-braces: HttpUrlDestinationPropertiesTypeDef](./type_defs.md#httpurldestinationpropertiestypedef) 
3. See [:material-code-braces: VpcDestinationPropertiesTypeDef](./type_defs.md#vpcdestinationpropertiestypedef) 
## ValidateSecurityProfileBehaviorsResponseTypeDef

```python
# ValidateSecurityProfileBehaviorsResponseTypeDef definition

class ValidateSecurityProfileBehaviorsResponseTypeDef(TypedDict):
    valid: bool,
    validationErrors: List[ValidationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationErrorTypeDef](./type_defs.md#validationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMetricValuesResponseTypeDef

```python
# ListMetricValuesResponseTypeDef definition

class ListMetricValuesResponseTypeDef(TypedDict):
    metricDatumList: List[MetricDatumTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricDatumTypeDef](./type_defs.md#metricdatumtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MitigationActionParamsTypeDef

```python
# MitigationActionParamsTypeDef definition

class MitigationActionParamsTypeDef(TypedDict):
    updateDeviceCertificateParams: NotRequired[UpdateDeviceCertificateParamsTypeDef],  # (1)
    updateCACertificateParams: NotRequired[UpdateCACertificateParamsTypeDef],  # (2)
    addThingsToThingGroupParams: NotRequired[AddThingsToThingGroupParamsUnionTypeDef],  # (3)
    replaceDefaultPolicyVersionParams: NotRequired[ReplaceDefaultPolicyVersionParamsTypeDef],  # (4)
    enableIoTLoggingParams: NotRequired[EnableIoTLoggingParamsTypeDef],  # (5)
    publishFindingToSnsParams: NotRequired[PublishFindingToSnsParamsTypeDef],  # (6)
```

1. See [:material-code-braces: UpdateDeviceCertificateParamsTypeDef](./type_defs.md#updatedevicecertificateparamstypedef) 
2. See [:material-code-braces: UpdateCACertificateParamsTypeDef](./type_defs.md#updatecacertificateparamstypedef) 
3. See [:material-code-braces: AddThingsToThingGroupParamsTypeDef](./type_defs.md#addthingstothinggroupparamstypedef) [:material-code-braces: AddThingsToThingGroupParamsOutputTypeDef](./type_defs.md#addthingstothinggroupparamsoutputtypedef) 
4. See [:material-code-braces: ReplaceDefaultPolicyVersionParamsTypeDef](./type_defs.md#replacedefaultpolicyversionparamstypedef) 
5. See [:material-code-braces: EnableIoTLoggingParamsTypeDef](./type_defs.md#enableiotloggingparamstypedef) 
6. See [:material-code-braces: PublishFindingToSnsParamsTypeDef](./type_defs.md#publishfindingtosnsparamstypedef) 
## DeniedTypeDef

```python
# DeniedTypeDef definition

class DeniedTypeDef(TypedDict):
    implicitDeny: NotRequired[ImplicitDenyTypeDef],  # (1)
    explicitDeny: NotRequired[ExplicitDenyTypeDef],  # (2)
```

1. See [:material-code-braces: ImplicitDenyTypeDef](./type_defs.md#implicitdenytypedef) 
2. See [:material-code-braces: ExplicitDenyTypeDef](./type_defs.md#explicitdenytypedef) 
## PutAssetPropertyValueEntryOutputTypeDef

```python
# PutAssetPropertyValueEntryOutputTypeDef definition

class PutAssetPropertyValueEntryOutputTypeDef(TypedDict):
    propertyValues: List[AssetPropertyValueTypeDef],  # (1)
    entryId: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## PutAssetPropertyValueEntryTypeDef

```python
# PutAssetPropertyValueEntryTypeDef definition

class PutAssetPropertyValueEntryTypeDef(TypedDict):
    propertyValues: Sequence[AssetPropertyValueTypeDef],  # (1)
    entryId: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## ThingGroupPropertiesTypeDef

```python
# ThingGroupPropertiesTypeDef definition

class ThingGroupPropertiesTypeDef(TypedDict):
    thingGroupDescription: NotRequired[str],
    attributePayload: NotRequired[AttributePayloadUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) [:material-code-braces: AttributePayloadOutputTypeDef](./type_defs.md#attributepayloadoutputtypedef) 
## TestAuthorizationRequestRequestTypeDef

```python
# TestAuthorizationRequestRequestTypeDef definition

class TestAuthorizationRequestRequestTypeDef(TypedDict):
    authInfos: Sequence[AuthInfoUnionTypeDef],  # (1)
    principal: NotRequired[str],
    cognitoIdentityPoolId: NotRequired[str],
    clientId: NotRequired[str],
    policyNamesToAdd: NotRequired[Sequence[str]],
    policyNamesToSkip: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AuthInfoTypeDef](./type_defs.md#authinfotypedef) [:material-code-braces: AuthInfoOutputTypeDef](./type_defs.md#authinfooutputtypedef) 
## AwsJobExecutionsRolloutConfigTypeDef

```python
# AwsJobExecutionsRolloutConfigTypeDef definition

class AwsJobExecutionsRolloutConfigTypeDef(TypedDict):
    maximumPerMinute: NotRequired[int],
    exponentialRate: NotRequired[AwsJobExponentialRolloutRateTypeDef],  # (1)
```

1. See [:material-code-braces: AwsJobExponentialRolloutRateTypeDef](./type_defs.md#awsjobexponentialrolloutratetypedef) 
## BehaviorOutputTypeDef

```python
# BehaviorOutputTypeDef definition

class BehaviorOutputTypeDef(TypedDict):
    name: str,
    metric: NotRequired[str],
    metricDimension: NotRequired[MetricDimensionTypeDef],  # (1)
    criteria: NotRequired[BehaviorCriteriaOutputTypeDef],  # (2)
    suppressAlerts: NotRequired[bool],
    exportMetric: NotRequired[bool],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-braces: BehaviorCriteriaOutputTypeDef](./type_defs.md#behaviorcriteriaoutputtypedef) 
## TestInvokeAuthorizerRequestRequestTypeDef

```python
# TestInvokeAuthorizerRequestRequestTypeDef definition

class TestInvokeAuthorizerRequestRequestTypeDef(TypedDict):
    authorizerName: str,
    token: NotRequired[str],
    tokenSignature: NotRequired[str],
    httpContext: NotRequired[HttpContextTypeDef],  # (1)
    mqttContext: NotRequired[MqttContextTypeDef],  # (2)
    tlsContext: NotRequired[TlsContextTypeDef],  # (3)
```

1. See [:material-code-braces: HttpContextTypeDef](./type_defs.md#httpcontexttypedef) 
2. See [:material-code-braces: MqttContextTypeDef](./type_defs.md#mqttcontexttypedef) 
3. See [:material-code-braces: TlsContextTypeDef](./type_defs.md#tlscontexttypedef) 
## GetBucketsAggregationRequestRequestTypeDef

```python
# GetBucketsAggregationRequestRequestTypeDef definition

class GetBucketsAggregationRequestRequestTypeDef(TypedDict):
    queryString: str,
    aggregationField: str,
    bucketsAggregationType: BucketsAggregationTypeTypeDef,  # (1)
    indexName: NotRequired[str],
    queryVersion: NotRequired[str],
```

1. See [:material-code-braces: BucketsAggregationTypeTypeDef](./type_defs.md#bucketsaggregationtypetypedef) 
## DescribeCACertificateResponseTypeDef

```python
# DescribeCACertificateResponseTypeDef definition

class DescribeCACertificateResponseTypeDef(TypedDict):
    certificateDescription: CACertificateDescriptionTypeDef,  # (1)
    registrationConfig: RegistrationConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CACertificateDescriptionTypeDef](./type_defs.md#cacertificatedescriptiontypedef) 
2. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCertificateResponseTypeDef

```python
# DescribeCertificateResponseTypeDef definition

class DescribeCertificateResponseTypeDef(TypedDict):
    certificateDescription: CertificateDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateDescriptionTypeDef](./type_defs.md#certificatedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCommandResponseTypeDef

```python
# GetCommandResponseTypeDef definition

class GetCommandResponseTypeDef(TypedDict):
    commandId: str,
    commandArn: str,
    namespace: CommandNamespaceType,  # (1)
    displayName: str,
    description: str,
    mandatoryParameters: List[CommandParameterOutputTypeDef],  # (2)
    payload: CommandPayloadOutputTypeDef,  # (3)
    roleArn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    deprecated: bool,
    pendingDeletion: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-braces: CommandParameterOutputTypeDef](./type_defs.md#commandparameteroutputtypedef) 
3. See [:material-code-braces: CommandPayloadOutputTypeDef](./type_defs.md#commandpayloadoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDetectMitigationActionsTaskRequestRequestTypeDef

```python
# StartDetectMitigationActionsTaskRequestRequestTypeDef definition

class StartDetectMitigationActionsTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
    target: DetectMitigationActionsTaskTargetTypeDef,  # (1)
    actions: Sequence[str],
    clientRequestToken: str,
    violationEventOccurrenceRange: NotRequired[ViolationEventOccurrenceRangeTypeDef],  # (2)
    includeOnlyActiveViolations: NotRequired[bool],
    includeSuppressedAlerts: NotRequired[bool],
```

1. See [:material-code-braces: DetectMitigationActionsTaskTargetTypeDef](./type_defs.md#detectmitigationactionstasktargettypedef) 
2. See [:material-code-braces: ViolationEventOccurrenceRangeTypeDef](./type_defs.md#violationeventoccurrencerangetypedef) 
## StartSigningJobParameterTypeDef

```python
# StartSigningJobParameterTypeDef definition

class StartSigningJobParameterTypeDef(TypedDict):
    signingProfileParameter: NotRequired[SigningProfileParameterTypeDef],  # (1)
    signingProfileName: NotRequired[str],
    destination: NotRequired[DestinationTypeDef],  # (2)
```

1. See [:material-code-braces: SigningProfileParameterTypeDef](./type_defs.md#signingprofileparametertypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## JobExecutionsRolloutConfigTypeDef

```python
# JobExecutionsRolloutConfigTypeDef definition

class JobExecutionsRolloutConfigTypeDef(TypedDict):
    maximumPerMinute: NotRequired[int],
    exponentialRate: NotRequired[ExponentialRolloutRateTypeDef],  # (1)
```

1. See [:material-code-braces: ExponentialRolloutRateTypeDef](./type_defs.md#exponentialrolloutratetypedef) 
## CreatePackageVersionRequestRequestTypeDef

```python
# CreatePackageVersionRequestRequestTypeDef definition

class CreatePackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    description: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    artifact: NotRequired[PackageVersionArtifactTypeDef],  # (1)
    recipe: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PackageVersionArtifactTypeDef](./type_defs.md#packageversionartifacttypedef) 
## UpdatePackageVersionRequestRequestTypeDef

```python
# UpdatePackageVersionRequestRequestTypeDef definition

class UpdatePackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    description: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    artifact: NotRequired[PackageVersionArtifactTypeDef],  # (1)
    action: NotRequired[PackageVersionActionType],  # (2)
    recipe: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PackageVersionArtifactTypeDef](./type_defs.md#packageversionartifacttypedef) 
2. See [:material-code-brackets: PackageVersionActionType](./literals.md#packageversionactiontype) 
## AssociateSbomWithPackageVersionRequestRequestTypeDef

```python
# AssociateSbomWithPackageVersionRequestRequestTypeDef definition

class AssociateSbomWithPackageVersionRequestRequestTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    sbom: SbomTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SbomTypeDef](./type_defs.md#sbomtypedef) 
## AssociateSbomWithPackageVersionResponseTypeDef

```python
# AssociateSbomWithPackageVersionResponseTypeDef definition

class AssociateSbomWithPackageVersionResponseTypeDef(TypedDict):
    packageName: str,
    versionName: str,
    sbom: SbomTypeDef,  # (1)
    sbomValidationStatus: SbomValidationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SbomTypeDef](./type_defs.md#sbomtypedef) 
2. See [:material-code-brackets: SbomValidationStatusType](./literals.md#sbomvalidationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPackageVersionResponseTypeDef

```python
# GetPackageVersionResponseTypeDef definition

class GetPackageVersionResponseTypeDef(TypedDict):
    packageVersionArn: str,
    packageName: str,
    versionName: str,
    description: str,
    attributes: Dict[str, str],
    artifact: PackageVersionArtifactTypeDef,  # (1)
    status: PackageVersionStatusType,  # (2)
    errorReason: str,
    creationDate: datetime,
    lastModifiedDate: datetime,
    sbom: SbomTypeDef,  # (3)
    sbomValidationStatus: SbomValidationStatusType,  # (4)
    recipe: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: PackageVersionArtifactTypeDef](./type_defs.md#packageversionartifacttypedef) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-braces: SbomTypeDef](./type_defs.md#sbomtypedef) 
4. See [:material-code-brackets: SbomValidationStatusType](./literals.md#sbomvalidationstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamRequestRequestTypeDef

```python
# CreateStreamRequestRequestTypeDef definition

class CreateStreamRequestRequestTypeDef(TypedDict):
    streamId: str,
    files: Sequence[StreamFileTypeDef],  # (1)
    roleArn: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: StreamFileTypeDef](./type_defs.md#streamfiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StreamInfoTypeDef

```python
# StreamInfoTypeDef definition

class StreamInfoTypeDef(TypedDict):
    streamId: NotRequired[str],
    streamArn: NotRequired[str],
    streamVersion: NotRequired[int],
    description: NotRequired[str],
    files: NotRequired[List[StreamFileTypeDef]],  # (1)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: StreamFileTypeDef](./type_defs.md#streamfiletypedef) 
## UpdateStreamRequestRequestTypeDef

```python
# UpdateStreamRequestRequestTypeDef definition

class UpdateStreamRequestRequestTypeDef(TypedDict):
    streamId: str,
    description: NotRequired[str],
    files: NotRequired[Sequence[StreamFileTypeDef]],  # (1)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: StreamFileTypeDef](./type_defs.md#streamfiletypedef) 
## ThingIndexingConfigurationOutputTypeDef

```python
# ThingIndexingConfigurationOutputTypeDef definition

class ThingIndexingConfigurationOutputTypeDef(TypedDict):
    thingIndexingMode: ThingIndexingModeType,  # (1)
    thingConnectivityIndexingMode: NotRequired[ThingConnectivityIndexingModeType],  # (2)
    deviceDefenderIndexingMode: NotRequired[DeviceDefenderIndexingModeType],  # (3)
    namedShadowIndexingMode: NotRequired[NamedShadowIndexingModeType],  # (4)
    managedFields: NotRequired[List[FieldTypeDef]],  # (5)
    customFields: NotRequired[List[FieldTypeDef]],  # (5)
    filter: NotRequired[IndexingFilterOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: ThingIndexingModeType](./literals.md#thingindexingmodetype) 
2. See [:material-code-brackets: ThingConnectivityIndexingModeType](./literals.md#thingconnectivityindexingmodetype) 
3. See [:material-code-brackets: DeviceDefenderIndexingModeType](./literals.md#devicedefenderindexingmodetype) 
4. See [:material-code-brackets: NamedShadowIndexingModeType](./literals.md#namedshadowindexingmodetype) 
5. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
6. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
7. See [:material-code-braces: IndexingFilterOutputTypeDef](./type_defs.md#indexingfilteroutputtypedef) 
## DescribeThingGroupResponseTypeDef

```python
# DescribeThingGroupResponseTypeDef definition

class DescribeThingGroupResponseTypeDef(TypedDict):
    thingGroupName: str,
    thingGroupId: str,
    thingGroupArn: str,
    version: int,
    thingGroupProperties: ThingGroupPropertiesOutputTypeDef,  # (1)
    thingGroupMetadata: ThingGroupMetadataTypeDef,  # (2)
    indexName: str,
    queryString: str,
    queryVersion: str,
    status: DynamicGroupStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ThingGroupPropertiesOutputTypeDef](./type_defs.md#thinggrouppropertiesoutputtypedef) 
2. See [:material-code-braces: ThingGroupMetadataTypeDef](./type_defs.md#thinggroupmetadatatypedef) 
3. See [:material-code-brackets: DynamicGroupStatusType](./literals.md#dynamicgroupstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HttpActionOutputTypeDef

```python
# HttpActionOutputTypeDef definition

class HttpActionOutputTypeDef(TypedDict):
    url: str,
    confirmationUrl: NotRequired[str],
    headers: NotRequired[List[HttpActionHeaderTypeDef]],  # (1)
    auth: NotRequired[HttpAuthorizationTypeDef],  # (2)
```

1. See [:material-code-braces: HttpActionHeaderTypeDef](./type_defs.md#httpactionheadertypedef) 
2. See [:material-code-braces: HttpAuthorizationTypeDef](./type_defs.md#httpauthorizationtypedef) 
## HttpActionTypeDef

```python
# HttpActionTypeDef definition

class HttpActionTypeDef(TypedDict):
    url: str,
    confirmationUrl: NotRequired[str],
    headers: NotRequired[Sequence[HttpActionHeaderTypeDef]],  # (1)
    auth: NotRequired[HttpAuthorizationTypeDef],  # (2)
```

1. See [:material-code-braces: HttpActionHeaderTypeDef](./type_defs.md#httpactionheadertypedef) 
2. See [:material-code-braces: HttpAuthorizationTypeDef](./type_defs.md#httpauthorizationtypedef) 
## DescribeJobExecutionResponseTypeDef

```python
# DescribeJobExecutionResponseTypeDef definition

class DescribeJobExecutionResponseTypeDef(TypedDict):
    execution: JobExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobExecutionTypeDef](./type_defs.md#jobexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobExecutionsForJobResponseTypeDef

```python
# ListJobExecutionsForJobResponseTypeDef definition

class ListJobExecutionsForJobResponseTypeDef(TypedDict):
    executionSummaries: List[JobExecutionSummaryForJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobExecutionSummaryForJobTypeDef](./type_defs.md#jobexecutionsummaryforjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobExecutionsForThingResponseTypeDef

```python
# ListJobExecutionsForThingResponseTypeDef definition

class ListJobExecutionsForThingResponseTypeDef(TypedDict):
    executionSummaries: List[JobExecutionSummaryForThingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobExecutionSummaryForThingTypeDef](./type_defs.md#jobexecutionsummaryforthingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilesForTargetResponseTypeDef

```python
# ListSecurityProfilesForTargetResponseTypeDef definition

class ListSecurityProfilesForTargetResponseTypeDef(TypedDict):
    securityProfileTargetMappings: List[SecurityProfileTargetMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityProfileTargetMappingTypeDef](./type_defs.md#securityprofiletargetmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListV2LoggingLevelsResponseTypeDef

```python
# ListV2LoggingLevelsResponseTypeDef definition

class ListV2LoggingLevelsResponseTypeDef(TypedDict):
    logTargetConfigurations: List[LogTargetConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LogTargetConfigurationTypeDef](./type_defs.md#logtargetconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BehaviorCriteriaTypeDef

```python
# BehaviorCriteriaTypeDef definition

class BehaviorCriteriaTypeDef(TypedDict):
    comparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
    value: NotRequired[MetricValueUnionTypeDef],  # (2)
    durationSeconds: NotRequired[int],
    consecutiveDatapointsToAlarm: NotRequired[int],
    consecutiveDatapointsToClear: NotRequired[int],
    statisticalThreshold: NotRequired[StatisticalThresholdTypeDef],  # (3)
    mlDetectionConfig: NotRequired[MachineLearningDetectionConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 
3. See [:material-code-braces: StatisticalThresholdTypeDef](./type_defs.md#statisticalthresholdtypedef) 
4. See [:material-code-braces: MachineLearningDetectionConfigTypeDef](./type_defs.md#machinelearningdetectionconfigtypedef) 
## DescribeMitigationActionResponseTypeDef

```python
# DescribeMitigationActionResponseTypeDef definition

class DescribeMitigationActionResponseTypeDef(TypedDict):
    actionName: str,
    actionType: MitigationActionTypeType,  # (1)
    actionArn: str,
    actionId: str,
    roleArn: str,
    actionParams: MitigationActionParamsOutputTypeDef,  # (2)
    creationDate: datetime,
    lastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype) 
2. See [:material-code-braces: MitigationActionParamsOutputTypeDef](./type_defs.md#mitigationactionparamsoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MitigationActionTypeDef

```python
# MitigationActionTypeDef definition

class MitigationActionTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    roleArn: NotRequired[str],
    actionParams: NotRequired[MitigationActionParamsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MitigationActionParamsOutputTypeDef](./type_defs.md#mitigationactionparamsoutputtypedef) 
## ThingTypePropertiesOutputTypeDef

```python
# ThingTypePropertiesOutputTypeDef definition

class ThingTypePropertiesOutputTypeDef(TypedDict):
    thingTypeDescription: NotRequired[str],
    searchableAttributes: NotRequired[List[str]],
    mqtt5Configuration: NotRequired[Mqtt5ConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: Mqtt5ConfigurationOutputTypeDef](./type_defs.md#mqtt5configurationoutputtypedef) 
## RepublishActionOutputTypeDef

```python
# RepublishActionOutputTypeDef definition

class RepublishActionOutputTypeDef(TypedDict):
    roleArn: str,
    topic: str,
    qos: NotRequired[int],
    headers: NotRequired[MqttHeadersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MqttHeadersOutputTypeDef](./type_defs.md#mqttheadersoutputtypedef) 
## AuditSuppressionTypeDef

```python
# AuditSuppressionTypeDef definition

class AuditSuppressionTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    expirationDate: NotRequired[datetime],
    suppressIndefinitely: NotRequired[bool],
    description: NotRequired[str],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## CreateAuditSuppressionRequestRequestTypeDef

```python
# CreateAuditSuppressionRequestRequestTypeDef definition

class CreateAuditSuppressionRequestRequestTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    clientRequestToken: str,
    expirationDate: NotRequired[TimestampTypeDef],
    suppressIndefinitely: NotRequired[bool],
    description: NotRequired[str],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## DeleteAuditSuppressionRequestRequestTypeDef

```python
# DeleteAuditSuppressionRequestRequestTypeDef definition

class DeleteAuditSuppressionRequestRequestTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## DescribeAuditSuppressionRequestRequestTypeDef

```python
# DescribeAuditSuppressionRequestRequestTypeDef definition

class DescribeAuditSuppressionRequestRequestTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## DescribeAuditSuppressionResponseTypeDef

```python
# DescribeAuditSuppressionResponseTypeDef definition

class DescribeAuditSuppressionResponseTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    expirationDate: datetime,
    suppressIndefinitely: bool,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAuditFindingsRequestPaginateTypeDef

```python
# ListAuditFindingsRequestPaginateTypeDef definition

class ListAuditFindingsRequestPaginateTypeDef(TypedDict):
    taskId: NotRequired[str],
    checkName: NotRequired[str],
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (1)
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    listSuppressedFindings: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuditFindingsRequestRequestTypeDef

```python
# ListAuditFindingsRequestRequestTypeDef definition

class ListAuditFindingsRequestRequestTypeDef(TypedDict):
    taskId: NotRequired[str],
    checkName: NotRequired[str],
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    listSuppressedFindings: NotRequired[bool],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## ListAuditSuppressionsRequestPaginateTypeDef

```python
# ListAuditSuppressionsRequestPaginateTypeDef definition

class ListAuditSuppressionsRequestPaginateTypeDef(TypedDict):
    checkName: NotRequired[str],
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (1)
    ascendingOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAuditSuppressionsRequestRequestTypeDef

```python
# ListAuditSuppressionsRequestRequestTypeDef definition

class ListAuditSuppressionsRequestRequestTypeDef(TypedDict):
    checkName: NotRequired[str],
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (1)
    ascendingOrder: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## NonCompliantResourceTypeDef

```python
# NonCompliantResourceTypeDef definition

class NonCompliantResourceTypeDef(TypedDict):
    resourceType: NotRequired[ResourceTypeType],  # (1)
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (2)
    additionalInfo: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## RelatedResourceTypeDef

```python
# RelatedResourceTypeDef definition

class RelatedResourceTypeDef(TypedDict):
    resourceType: NotRequired[ResourceTypeType],  # (1)
    resourceIdentifier: NotRequired[ResourceIdentifierTypeDef],  # (2)
    additionalInfo: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## UpdateAuditSuppressionRequestRequestTypeDef

```python
# UpdateAuditSuppressionRequestRequestTypeDef definition

class UpdateAuditSuppressionRequestRequestTypeDef(TypedDict):
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    expirationDate: NotRequired[TimestampTypeDef],
    suppressIndefinitely: NotRequired[bool],
    description: NotRequired[str],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
## SearchIndexResponseTypeDef

```python
# SearchIndexResponseTypeDef definition

class SearchIndexResponseTypeDef(TypedDict):
    things: List[ThingDocumentTypeDef],  # (1)
    thingGroups: List[ThingGroupDocumentTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ThingDocumentTypeDef](./type_defs.md#thingdocumenttypedef) 
2. See [:material-code-braces: ThingGroupDocumentTypeDef](./type_defs.md#thinggroupdocumenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicRuleDestinationRequestRequestTypeDef

```python
# CreateTopicRuleDestinationRequestRequestTypeDef definition

class CreateTopicRuleDestinationRequestRequestTypeDef(TypedDict):
    destinationConfiguration: TopicRuleDestinationConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TopicRuleDestinationConfigurationTypeDef](./type_defs.md#topicruledestinationconfigurationtypedef) 
## ListTopicRuleDestinationsResponseTypeDef

```python
# ListTopicRuleDestinationsResponseTypeDef definition

class ListTopicRuleDestinationsResponseTypeDef(TypedDict):
    destinationSummaries: List[TopicRuleDestinationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TopicRuleDestinationSummaryTypeDef](./type_defs.md#topicruledestinationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicRuleDestinationResponseTypeDef

```python
# CreateTopicRuleDestinationResponseTypeDef definition

class CreateTopicRuleDestinationResponseTypeDef(TypedDict):
    topicRuleDestination: TopicRuleDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRuleDestinationTypeDef](./type_defs.md#topicruledestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTopicRuleDestinationResponseTypeDef

```python
# GetTopicRuleDestinationResponseTypeDef definition

class GetTopicRuleDestinationResponseTypeDef(TypedDict):
    topicRuleDestination: TopicRuleDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRuleDestinationTypeDef](./type_defs.md#topicruledestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMitigationActionRequestRequestTypeDef

```python
# CreateMitigationActionRequestRequestTypeDef definition

class CreateMitigationActionRequestRequestTypeDef(TypedDict):
    actionName: str,
    roleArn: str,
    actionParams: MitigationActionParamsTypeDef,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: MitigationActionParamsTypeDef](./type_defs.md#mitigationactionparamstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateMitigationActionRequestRequestTypeDef

```python
# UpdateMitigationActionRequestRequestTypeDef definition

class UpdateMitigationActionRequestRequestTypeDef(TypedDict):
    actionName: str,
    roleArn: NotRequired[str],
    actionParams: NotRequired[MitigationActionParamsTypeDef],  # (1)
```

1. See [:material-code-braces: MitigationActionParamsTypeDef](./type_defs.md#mitigationactionparamstypedef) 
## AuthResultTypeDef

```python
# AuthResultTypeDef definition

class AuthResultTypeDef(TypedDict):
    authInfo: NotRequired[AuthInfoOutputTypeDef],  # (1)
    allowed: NotRequired[AllowedTypeDef],  # (2)
    denied: NotRequired[DeniedTypeDef],  # (3)
    authDecision: NotRequired[AuthDecisionType],  # (4)
    missingContextValues: NotRequired[List[str]],
```

1. See [:material-code-braces: AuthInfoOutputTypeDef](./type_defs.md#authinfooutputtypedef) 
2. See [:material-code-braces: AllowedTypeDef](./type_defs.md#allowedtypedef) 
3. See [:material-code-braces: DeniedTypeDef](./type_defs.md#deniedtypedef) 
4. See [:material-code-brackets: AuthDecisionType](./literals.md#authdecisiontype) 
## IotSiteWiseActionOutputTypeDef

```python
# IotSiteWiseActionOutputTypeDef definition

class IotSiteWiseActionOutputTypeDef(TypedDict):
    putAssetPropertyValueEntries: List[PutAssetPropertyValueEntryOutputTypeDef],  # (1)
    roleArn: str,
```

1. See [:material-code-braces: PutAssetPropertyValueEntryOutputTypeDef](./type_defs.md#putassetpropertyvalueentryoutputtypedef) 
## CreateDynamicThingGroupRequestRequestTypeDef

```python
# CreateDynamicThingGroupRequestRequestTypeDef definition

class CreateDynamicThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    queryString: str,
    thingGroupProperties: NotRequired[ThingGroupPropertiesTypeDef],  # (1)
    indexName: NotRequired[str],
    queryVersion: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateThingGroupRequestRequestTypeDef

```python
# CreateThingGroupRequestRequestTypeDef definition

class CreateThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    parentGroupName: NotRequired[str],
    thingGroupProperties: NotRequired[ThingGroupPropertiesTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDynamicThingGroupRequestRequestTypeDef

```python
# UpdateDynamicThingGroupRequestRequestTypeDef definition

class UpdateDynamicThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    thingGroupProperties: ThingGroupPropertiesTypeDef,  # (1)
    expectedVersion: NotRequired[int],
    indexName: NotRequired[str],
    queryString: NotRequired[str],
    queryVersion: NotRequired[str],
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
## UpdateThingGroupRequestRequestTypeDef

```python
# UpdateThingGroupRequestRequestTypeDef definition

class UpdateThingGroupRequestRequestTypeDef(TypedDict):
    thingGroupName: str,
    thingGroupProperties: ThingGroupPropertiesTypeDef,  # (1)
    expectedVersion: NotRequired[int],
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
## ActiveViolationTypeDef

```python
# ActiveViolationTypeDef definition

class ActiveViolationTypeDef(TypedDict):
    violationId: NotRequired[str],
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behavior: NotRequired[BehaviorOutputTypeDef],  # (1)
    lastViolationValue: NotRequired[MetricValueOutputTypeDef],  # (2)
    violationEventAdditionalInfo: NotRequired[ViolationEventAdditionalInfoTypeDef],  # (3)
    verificationState: NotRequired[VerificationStateType],  # (4)
    verificationStateDescription: NotRequired[str],
    lastViolationTime: NotRequired[datetime],
    violationStartTime: NotRequired[datetime],
```

1. See [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 
3. See [:material-code-braces: ViolationEventAdditionalInfoTypeDef](./type_defs.md#violationeventadditionalinfotypedef) 
4. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
## DescribeSecurityProfileResponseTypeDef

```python
# DescribeSecurityProfileResponseTypeDef definition

class DescribeSecurityProfileResponseTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileArn: str,
    securityProfileDescription: str,
    behaviors: List[BehaviorOutputTypeDef],  # (1)
    alertTargets: Dict[AlertTargetTypeType, AlertTargetTypeDef],  # (2)
    additionalMetricsToRetain: List[str],
    additionalMetricsToRetainV2: List[MetricToRetainTypeDef],  # (3)
    version: int,
    creationDate: datetime,
    lastModifiedDate: datetime,
    metricsExportConfig: MetricsExportConfigTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityProfileResponseTypeDef

```python
# UpdateSecurityProfileResponseTypeDef definition

class UpdateSecurityProfileResponseTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileArn: str,
    securityProfileDescription: str,
    behaviors: List[BehaviorOutputTypeDef],  # (1)
    alertTargets: Dict[AlertTargetTypeType, AlertTargetTypeDef],  # (2)
    additionalMetricsToRetain: List[str],
    additionalMetricsToRetainV2: List[MetricToRetainTypeDef],  # (3)
    version: int,
    creationDate: datetime,
    lastModifiedDate: datetime,
    metricsExportConfig: MetricsExportConfigTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ViolationEventTypeDef

```python
# ViolationEventTypeDef definition

class ViolationEventTypeDef(TypedDict):
    violationId: NotRequired[str],
    thingName: NotRequired[str],
    securityProfileName: NotRequired[str],
    behavior: NotRequired[BehaviorOutputTypeDef],  # (1)
    metricValue: NotRequired[MetricValueOutputTypeDef],  # (2)
    violationEventAdditionalInfo: NotRequired[ViolationEventAdditionalInfoTypeDef],  # (3)
    violationEventType: NotRequired[ViolationEventTypeType],  # (4)
    verificationState: NotRequired[VerificationStateType],  # (5)
    verificationStateDescription: NotRequired[str],
    violationEventTime: NotRequired[datetime],
```

1. See [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-braces: MetricValueOutputTypeDef](./type_defs.md#metricvalueoutputtypedef) 
3. See [:material-code-braces: ViolationEventAdditionalInfoTypeDef](./type_defs.md#violationeventadditionalinfotypedef) 
4. See [:material-code-brackets: ViolationEventTypeType](./literals.md#violationeventtypetype) 
5. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
## CustomCodeSigningTypeDef

```python
# CustomCodeSigningTypeDef definition

class CustomCodeSigningTypeDef(TypedDict):
    signature: NotRequired[CodeSigningSignatureUnionTypeDef],  # (1)
    certificateChain: NotRequired[CodeSigningCertificateChainTypeDef],  # (2)
    hashAlgorithm: NotRequired[str],
    signatureAlgorithm: NotRequired[str],
```

1. See [:material-code-braces: CodeSigningSignatureTypeDef](./type_defs.md#codesigningsignaturetypedef) [:material-code-braces: CodeSigningSignatureOutputTypeDef](./type_defs.md#codesigningsignatureoutputtypedef) 
2. See [:material-code-braces: CodeSigningCertificateChainTypeDef](./type_defs.md#codesigningcertificatechaintypedef) 
## CommandParameterTypeDef

```python
# CommandParameterTypeDef definition

class CommandParameterTypeDef(TypedDict):
    name: str,
    value: NotRequired[CommandParameterValueUnionTypeDef],  # (1)
    defaultValue: NotRequired[CommandParameterValueUnionTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: CommandParameterValueTypeDef](./type_defs.md#commandparametervaluetypedef) [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 
2. See [:material-code-braces: CommandParameterValueTypeDef](./type_defs.md#commandparametervaluetypedef) [:material-code-braces: CommandParameterValueOutputTypeDef](./type_defs.md#commandparametervalueoutputtypedef) 
## CodeSigningOutputTypeDef

```python
# CodeSigningOutputTypeDef definition

class CodeSigningOutputTypeDef(TypedDict):
    awsSignerJobId: NotRequired[str],
    startSigningJobParameter: NotRequired[StartSigningJobParameterTypeDef],  # (1)
    customCodeSigning: NotRequired[CustomCodeSigningOutputTypeDef],  # (2)
```

1. See [:material-code-braces: StartSigningJobParameterTypeDef](./type_defs.md#startsigningjobparametertypedef) 
2. See [:material-code-braces: CustomCodeSigningOutputTypeDef](./type_defs.md#customcodesigningoutputtypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    targets: Sequence[str],
    documentSource: NotRequired[str],
    document: NotRequired[str],
    description: NotRequired[str],
    presignedUrlConfig: NotRequired[PresignedUrlConfigTypeDef],  # (1)
    targetSelection: NotRequired[TargetSelectionType],  # (2)
    jobExecutionsRolloutConfig: NotRequired[JobExecutionsRolloutConfigTypeDef],  # (3)
    abortConfig: NotRequired[AbortConfigTypeDef],  # (4)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (5)
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    namespaceId: NotRequired[str],
    jobTemplateArn: NotRequired[str],
    jobExecutionsRetryConfig: NotRequired[JobExecutionsRetryConfigTypeDef],  # (7)
    documentParameters: NotRequired[Mapping[str, str]],
    schedulingConfig: NotRequired[SchedulingConfigTypeDef],  # (8)
    destinationPackageVersions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
3. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
4. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
5. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
8. See [:material-code-braces: SchedulingConfigTypeDef](./type_defs.md#schedulingconfigtypedef) 
## CreateJobTemplateRequestRequestTypeDef

```python
# CreateJobTemplateRequestRequestTypeDef definition

class CreateJobTemplateRequestRequestTypeDef(TypedDict):
    jobTemplateId: str,
    description: str,
    jobArn: NotRequired[str],
    documentSource: NotRequired[str],
    document: NotRequired[str],
    presignedUrlConfig: NotRequired[PresignedUrlConfigTypeDef],  # (1)
    jobExecutionsRolloutConfig: NotRequired[JobExecutionsRolloutConfigTypeDef],  # (2)
    abortConfig: NotRequired[AbortConfigTypeDef],  # (3)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (4)
    tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    jobExecutionsRetryConfig: NotRequired[JobExecutionsRetryConfigTypeDef],  # (6)
    maintenanceWindows: NotRequired[Sequence[MaintenanceWindowTypeDef]],  # (7)
    destinationPackageVersions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
4. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
7. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
## DescribeJobTemplateResponseTypeDef

```python
# DescribeJobTemplateResponseTypeDef definition

class DescribeJobTemplateResponseTypeDef(TypedDict):
    jobTemplateArn: str,
    jobTemplateId: str,
    description: str,
    documentSource: str,
    document: str,
    createdAt: datetime,
    presignedUrlConfig: PresignedUrlConfigTypeDef,  # (1)
    jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef,  # (2)
    abortConfig: AbortConfigOutputTypeDef,  # (3)
    timeoutConfig: TimeoutConfigTypeDef,  # (4)
    jobExecutionsRetryConfig: JobExecutionsRetryConfigOutputTypeDef,  # (5)
    maintenanceWindows: List[MaintenanceWindowTypeDef],  # (6)
    destinationPackageVersions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AbortConfigOutputTypeDef](./type_defs.md#abortconfigoutputtypedef) 
4. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
5. See [:material-code-braces: JobExecutionsRetryConfigOutputTypeDef](./type_defs.md#jobexecutionsretryconfigoutputtypedef) 
6. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    jobArn: NotRequired[str],
    jobId: NotRequired[str],
    targetSelection: NotRequired[TargetSelectionType],  # (1)
    status: NotRequired[JobStatusType],  # (2)
    forceCanceled: NotRequired[bool],
    reasonCode: NotRequired[str],
    comment: NotRequired[str],
    targets: NotRequired[List[str]],
    description: NotRequired[str],
    presignedUrlConfig: NotRequired[PresignedUrlConfigTypeDef],  # (3)
    jobExecutionsRolloutConfig: NotRequired[JobExecutionsRolloutConfigTypeDef],  # (4)
    abortConfig: NotRequired[AbortConfigOutputTypeDef],  # (5)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    completedAt: NotRequired[datetime],
    jobProcessDetails: NotRequired[JobProcessDetailsTypeDef],  # (6)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (7)
    namespaceId: NotRequired[str],
    jobTemplateArn: NotRequired[str],
    jobExecutionsRetryConfig: NotRequired[JobExecutionsRetryConfigOutputTypeDef],  # (8)
    documentParameters: NotRequired[Dict[str, str]],
    isConcurrent: NotRequired[bool],
    schedulingConfig: NotRequired[SchedulingConfigOutputTypeDef],  # (9)
    scheduledJobRollouts: NotRequired[List[ScheduledJobRolloutTypeDef]],  # (10)
    destinationPackageVersions: NotRequired[List[str]],
```

1. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
4. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
5. See [:material-code-braces: AbortConfigOutputTypeDef](./type_defs.md#abortconfigoutputtypedef) 
6. See [:material-code-braces: JobProcessDetailsTypeDef](./type_defs.md#jobprocessdetailstypedef) 
7. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
8. See [:material-code-braces: JobExecutionsRetryConfigOutputTypeDef](./type_defs.md#jobexecutionsretryconfigoutputtypedef) 
9. See [:material-code-braces: SchedulingConfigOutputTypeDef](./type_defs.md#schedulingconfigoutputtypedef) 
10. See [:material-code-braces: ScheduledJobRolloutTypeDef](./type_defs.md#scheduledjobrollouttypedef) 
## UpdateJobRequestRequestTypeDef

```python
# UpdateJobRequestRequestTypeDef definition

class UpdateJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    description: NotRequired[str],
    presignedUrlConfig: NotRequired[PresignedUrlConfigTypeDef],  # (1)
    jobExecutionsRolloutConfig: NotRequired[JobExecutionsRolloutConfigTypeDef],  # (2)
    abortConfig: NotRequired[AbortConfigTypeDef],  # (3)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (4)
    namespaceId: NotRequired[str],
    jobExecutionsRetryConfig: NotRequired[JobExecutionsRetryConfigTypeDef],  # (5)
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
4. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
5. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
## DescribeStreamResponseTypeDef

```python
# DescribeStreamResponseTypeDef definition

class DescribeStreamResponseTypeDef(TypedDict):
    streamInfo: StreamInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamInfoTypeDef](./type_defs.md#streaminfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIndexingConfigurationResponseTypeDef

```python
# GetIndexingConfigurationResponseTypeDef definition

class GetIndexingConfigurationResponseTypeDef(TypedDict):
    thingIndexingConfiguration: ThingIndexingConfigurationOutputTypeDef,  # (1)
    thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ThingIndexingConfigurationOutputTypeDef](./type_defs.md#thingindexingconfigurationoutputtypedef) 
2. See [:material-code-braces: ThingGroupIndexingConfigurationOutputTypeDef](./type_defs.md#thinggroupindexingconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThingIndexingConfigurationTypeDef

```python
# ThingIndexingConfigurationTypeDef definition

class ThingIndexingConfigurationTypeDef(TypedDict):
    thingIndexingMode: ThingIndexingModeType,  # (1)
    thingConnectivityIndexingMode: NotRequired[ThingConnectivityIndexingModeType],  # (2)
    deviceDefenderIndexingMode: NotRequired[DeviceDefenderIndexingModeType],  # (3)
    namedShadowIndexingMode: NotRequired[NamedShadowIndexingModeType],  # (4)
    managedFields: NotRequired[Sequence[FieldTypeDef]],  # (5)
    customFields: NotRequired[Sequence[FieldTypeDef]],  # (5)
    filter: NotRequired[IndexingFilterUnionTypeDef],  # (7)
```

1. See [:material-code-brackets: ThingIndexingModeType](./literals.md#thingindexingmodetype) 
2. See [:material-code-brackets: ThingConnectivityIndexingModeType](./literals.md#thingconnectivityindexingmodetype) 
3. See [:material-code-brackets: DeviceDefenderIndexingModeType](./literals.md#devicedefenderindexingmodetype) 
4. See [:material-code-brackets: NamedShadowIndexingModeType](./literals.md#namedshadowindexingmodetype) 
5. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
6. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
7. See [:material-code-braces: IndexingFilterTypeDef](./type_defs.md#indexingfiltertypedef) [:material-code-braces: IndexingFilterOutputTypeDef](./type_defs.md#indexingfilteroutputtypedef) 
## DescribeAuditMitigationActionsTaskResponseTypeDef

```python
# DescribeAuditMitigationActionsTaskResponseTypeDef definition

class DescribeAuditMitigationActionsTaskResponseTypeDef(TypedDict):
    taskStatus: AuditMitigationActionsTaskStatusType,  # (1)
    startTime: datetime,
    endTime: datetime,
    taskStatistics: Dict[str, TaskStatisticsForAuditCheckTypeDef],  # (2)
    target: AuditMitigationActionsTaskTargetOutputTypeDef,  # (3)
    auditCheckToActionsMapping: Dict[str, List[str]],
    actionsDefinition: List[MitigationActionTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
2. See [:material-code-braces: TaskStatisticsForAuditCheckTypeDef](./type_defs.md#taskstatisticsforauditchecktypedef) 
3. See [:material-code-braces: AuditMitigationActionsTaskTargetOutputTypeDef](./type_defs.md#auditmitigationactionstasktargetoutputtypedef) 
4. See [:material-code-braces: MitigationActionTypeDef](./type_defs.md#mitigationactiontypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectMitigationActionsTaskSummaryTypeDef

```python
# DetectMitigationActionsTaskSummaryTypeDef definition

class DetectMitigationActionsTaskSummaryTypeDef(TypedDict):
    taskId: NotRequired[str],
    taskStatus: NotRequired[DetectMitigationActionsTaskStatusType],  # (1)
    taskStartTime: NotRequired[datetime],
    taskEndTime: NotRequired[datetime],
    target: NotRequired[DetectMitigationActionsTaskTargetOutputTypeDef],  # (2)
    violationEventOccurrenceRange: NotRequired[ViolationEventOccurrenceRangeOutputTypeDef],  # (3)
    onlyActiveViolationsIncluded: NotRequired[bool],
    suppressedAlertsIncluded: NotRequired[bool],
    actionsDefinition: NotRequired[List[MitigationActionTypeDef]],  # (4)
    taskStatistics: NotRequired[DetectMitigationActionsTaskStatisticsTypeDef],  # (5)
```

1. See [:material-code-brackets: DetectMitigationActionsTaskStatusType](./literals.md#detectmitigationactionstaskstatustype) 
2. See [:material-code-braces: DetectMitigationActionsTaskTargetOutputTypeDef](./type_defs.md#detectmitigationactionstasktargetoutputtypedef) 
3. See [:material-code-braces: ViolationEventOccurrenceRangeOutputTypeDef](./type_defs.md#violationeventoccurrencerangeoutputtypedef) 
4. See [:material-code-braces: MitigationActionTypeDef](./type_defs.md#mitigationactiontypedef) 
5. See [:material-code-braces: DetectMitigationActionsTaskStatisticsTypeDef](./type_defs.md#detectmitigationactionstaskstatisticstypedef) 
## DescribeThingTypeResponseTypeDef

```python
# DescribeThingTypeResponseTypeDef definition

class DescribeThingTypeResponseTypeDef(TypedDict):
    thingTypeName: str,
    thingTypeId: str,
    thingTypeArn: str,
    thingTypeProperties: ThingTypePropertiesOutputTypeDef,  # (1)
    thingTypeMetadata: ThingTypeMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ThingTypePropertiesOutputTypeDef](./type_defs.md#thingtypepropertiesoutputtypedef) 
2. See [:material-code-braces: ThingTypeMetadataTypeDef](./type_defs.md#thingtypemetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThingTypeDefinitionTypeDef

```python
# ThingTypeDefinitionTypeDef definition

class ThingTypeDefinitionTypeDef(TypedDict):
    thingTypeName: NotRequired[str],
    thingTypeArn: NotRequired[str],
    thingTypeProperties: NotRequired[ThingTypePropertiesOutputTypeDef],  # (1)
    thingTypeMetadata: NotRequired[ThingTypeMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: ThingTypePropertiesOutputTypeDef](./type_defs.md#thingtypepropertiesoutputtypedef) 
2. See [:material-code-braces: ThingTypeMetadataTypeDef](./type_defs.md#thingtypemetadatatypedef) 
## ThingTypePropertiesTypeDef

```python
# ThingTypePropertiesTypeDef definition

class ThingTypePropertiesTypeDef(TypedDict):
    thingTypeDescription: NotRequired[str],
    searchableAttributes: NotRequired[Sequence[str]],
    mqtt5Configuration: NotRequired[Mqtt5ConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: Mqtt5ConfigurationTypeDef](./type_defs.md#mqtt5configurationtypedef) [:material-code-braces: Mqtt5ConfigurationOutputTypeDef](./type_defs.md#mqtt5configurationoutputtypedef) 
## RepublishActionTypeDef

```python
# RepublishActionTypeDef definition

class RepublishActionTypeDef(TypedDict):
    roleArn: str,
    topic: str,
    qos: NotRequired[int],
    headers: NotRequired[MqttHeadersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: MqttHeadersTypeDef](./type_defs.md#mqttheaderstypedef) [:material-code-braces: MqttHeadersOutputTypeDef](./type_defs.md#mqttheadersoutputtypedef) 
## ListAuditSuppressionsResponseTypeDef

```python
# ListAuditSuppressionsResponseTypeDef definition

class ListAuditSuppressionsResponseTypeDef(TypedDict):
    suppressions: List[AuditSuppressionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditSuppressionTypeDef](./type_defs.md#auditsuppressiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuditFindingTypeDef

```python
# AuditFindingTypeDef definition

class AuditFindingTypeDef(TypedDict):
    findingId: NotRequired[str],
    taskId: NotRequired[str],
    checkName: NotRequired[str],
    taskStartTime: NotRequired[datetime],
    findingTime: NotRequired[datetime],
    severity: NotRequired[AuditFindingSeverityType],  # (1)
    nonCompliantResource: NotRequired[NonCompliantResourceTypeDef],  # (2)
    relatedResources: NotRequired[List[RelatedResourceTypeDef]],  # (3)
    reasonForNonCompliance: NotRequired[str],
    reasonForNonComplianceCode: NotRequired[str],
    isSuppressed: NotRequired[bool],
```

1. See [:material-code-brackets: AuditFindingSeverityType](./literals.md#auditfindingseveritytype) 
2. See [:material-code-braces: NonCompliantResourceTypeDef](./type_defs.md#noncompliantresourcetypedef) 
3. See [:material-code-braces: RelatedResourceTypeDef](./type_defs.md#relatedresourcetypedef) 
## ListRelatedResourcesForAuditFindingResponseTypeDef

```python
# ListRelatedResourcesForAuditFindingResponseTypeDef definition

class ListRelatedResourcesForAuditFindingResponseTypeDef(TypedDict):
    relatedResources: List[RelatedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RelatedResourceTypeDef](./type_defs.md#relatedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestAuthorizationResponseTypeDef

```python
# TestAuthorizationResponseTypeDef definition

class TestAuthorizationResponseTypeDef(TypedDict):
    authResults: List[AuthResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthResultTypeDef](./type_defs.md#authresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionOutputTypeDef

```python
# ActionOutputTypeDef definition

class ActionOutputTypeDef(TypedDict):
    dynamoDB: NotRequired[DynamoDBActionTypeDef],  # (1)
    dynamoDBv2: NotRequired[DynamoDBv2ActionTypeDef],  # (2)
    lambda: NotRequired[LambdaActionTypeDef],  # (3)
    sns: NotRequired[SnsActionTypeDef],  # (4)
    sqs: NotRequired[SqsActionTypeDef],  # (5)
    kinesis: NotRequired[KinesisActionTypeDef],  # (6)
    republish: NotRequired[RepublishActionOutputTypeDef],  # (7)
    s3: NotRequired[S3ActionTypeDef],  # (8)
    firehose: NotRequired[FirehoseActionTypeDef],  # (9)
    cloudwatchMetric: NotRequired[CloudwatchMetricActionTypeDef],  # (10)
    cloudwatchAlarm: NotRequired[CloudwatchAlarmActionTypeDef],  # (11)
    cloudwatchLogs: NotRequired[CloudwatchLogsActionTypeDef],  # (12)
    elasticsearch: NotRequired[ElasticsearchActionTypeDef],  # (13)
    salesforce: NotRequired[SalesforceActionTypeDef],  # (14)
    iotAnalytics: NotRequired[IotAnalyticsActionTypeDef],  # (15)
    iotEvents: NotRequired[IotEventsActionTypeDef],  # (16)
    iotSiteWise: NotRequired[IotSiteWiseActionOutputTypeDef],  # (17)
    stepFunctions: NotRequired[StepFunctionsActionTypeDef],  # (18)
    timestream: NotRequired[TimestreamActionOutputTypeDef],  # (19)
    http: NotRequired[HttpActionOutputTypeDef],  # (20)
    kafka: NotRequired[KafkaActionOutputTypeDef],  # (21)
    openSearch: NotRequired[OpenSearchActionTypeDef],  # (22)
    location: NotRequired[LocationActionTypeDef],  # (23)
```

1. See [:material-code-braces: DynamoDBActionTypeDef](./type_defs.md#dynamodbactiontypedef) 
2. See [:material-code-braces: DynamoDBv2ActionTypeDef](./type_defs.md#dynamodbv2actiontypedef) 
3. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
4. See [:material-code-braces: SnsActionTypeDef](./type_defs.md#snsactiontypedef) 
5. See [:material-code-braces: SqsActionTypeDef](./type_defs.md#sqsactiontypedef) 
6. See [:material-code-braces: KinesisActionTypeDef](./type_defs.md#kinesisactiontypedef) 
7. See [:material-code-braces: RepublishActionOutputTypeDef](./type_defs.md#republishactionoutputtypedef) 
8. See [:material-code-braces: S3ActionTypeDef](./type_defs.md#s3actiontypedef) 
9. See [:material-code-braces: FirehoseActionTypeDef](./type_defs.md#firehoseactiontypedef) 
10. See [:material-code-braces: CloudwatchMetricActionTypeDef](./type_defs.md#cloudwatchmetricactiontypedef) 
11. See [:material-code-braces: CloudwatchAlarmActionTypeDef](./type_defs.md#cloudwatchalarmactiontypedef) 
12. See [:material-code-braces: CloudwatchLogsActionTypeDef](./type_defs.md#cloudwatchlogsactiontypedef) 
13. See [:material-code-braces: ElasticsearchActionTypeDef](./type_defs.md#elasticsearchactiontypedef) 
14. See [:material-code-braces: SalesforceActionTypeDef](./type_defs.md#salesforceactiontypedef) 
15. See [:material-code-braces: IotAnalyticsActionTypeDef](./type_defs.md#iotanalyticsactiontypedef) 
16. See [:material-code-braces: IotEventsActionTypeDef](./type_defs.md#ioteventsactiontypedef) 
17. See [:material-code-braces: IotSiteWiseActionOutputTypeDef](./type_defs.md#iotsitewiseactionoutputtypedef) 
18. See [:material-code-braces: StepFunctionsActionTypeDef](./type_defs.md#stepfunctionsactiontypedef) 
19. See [:material-code-braces: TimestreamActionOutputTypeDef](./type_defs.md#timestreamactionoutputtypedef) 
20. See [:material-code-braces: HttpActionOutputTypeDef](./type_defs.md#httpactionoutputtypedef) 
21. See [:material-code-braces: KafkaActionOutputTypeDef](./type_defs.md#kafkaactionoutputtypedef) 
22. See [:material-code-braces: OpenSearchActionTypeDef](./type_defs.md#opensearchactiontypedef) 
23. See [:material-code-braces: LocationActionTypeDef](./type_defs.md#locationactiontypedef) 
## IotSiteWiseActionTypeDef

```python
# IotSiteWiseActionTypeDef definition

class IotSiteWiseActionTypeDef(TypedDict):
    putAssetPropertyValueEntries: Sequence[PutAssetPropertyValueEntryUnionTypeDef],  # (1)
    roleArn: str,
```

1. See [:material-code-braces: PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef) [:material-code-braces: PutAssetPropertyValueEntryOutputTypeDef](./type_defs.md#putassetpropertyvalueentryoutputtypedef) 
## ListActiveViolationsResponseTypeDef

```python
# ListActiveViolationsResponseTypeDef definition

class ListActiveViolationsResponseTypeDef(TypedDict):
    activeViolations: List[ActiveViolationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActiveViolationTypeDef](./type_defs.md#activeviolationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViolationEventsResponseTypeDef

```python
# ListViolationEventsResponseTypeDef definition

class ListViolationEventsResponseTypeDef(TypedDict):
    violationEvents: List[ViolationEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ViolationEventTypeDef](./type_defs.md#violationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OTAUpdateFileOutputTypeDef

```python
# OTAUpdateFileOutputTypeDef definition

class OTAUpdateFileOutputTypeDef(TypedDict):
    fileName: NotRequired[str],
    fileType: NotRequired[int],
    fileVersion: NotRequired[str],
    fileLocation: NotRequired[FileLocationTypeDef],  # (1)
    codeSigning: NotRequired[CodeSigningOutputTypeDef],  # (2)
    attributes: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FileLocationTypeDef](./type_defs.md#filelocationtypedef) 
2. See [:material-code-braces: CodeSigningOutputTypeDef](./type_defs.md#codesigningoutputtypedef) 
## DescribeJobResponseTypeDef

```python
# DescribeJobResponseTypeDef definition

class DescribeJobResponseTypeDef(TypedDict):
    documentSource: str,
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIndexingConfigurationRequestRequestTypeDef

```python
# UpdateIndexingConfigurationRequestRequestTypeDef definition

class UpdateIndexingConfigurationRequestRequestTypeDef(TypedDict):
    thingIndexingConfiguration: NotRequired[ThingIndexingConfigurationTypeDef],  # (1)
    thingGroupIndexingConfiguration: NotRequired[ThingGroupIndexingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ThingIndexingConfigurationTypeDef](./type_defs.md#thingindexingconfigurationtypedef) 
2. See [:material-code-braces: ThingGroupIndexingConfigurationTypeDef](./type_defs.md#thinggroupindexingconfigurationtypedef) 
## BehaviorTypeDef

```python
# BehaviorTypeDef definition

class BehaviorTypeDef(TypedDict):
    name: str,
    metric: NotRequired[str],
    metricDimension: NotRequired[MetricDimensionTypeDef],  # (1)
    criteria: NotRequired[BehaviorCriteriaUnionTypeDef],  # (2)
    suppressAlerts: NotRequired[bool],
    exportMetric: NotRequired[bool],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-braces: BehaviorCriteriaTypeDef](./type_defs.md#behaviorcriteriatypedef) [:material-code-braces: BehaviorCriteriaOutputTypeDef](./type_defs.md#behaviorcriteriaoutputtypedef) 
## DescribeDetectMitigationActionsTaskResponseTypeDef

```python
# DescribeDetectMitigationActionsTaskResponseTypeDef definition

class DescribeDetectMitigationActionsTaskResponseTypeDef(TypedDict):
    taskSummary: DetectMitigationActionsTaskSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectMitigationActionsTaskSummaryTypeDef](./type_defs.md#detectmitigationactionstasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDetectMitigationActionsTasksResponseTypeDef

```python
# ListDetectMitigationActionsTasksResponseTypeDef definition

class ListDetectMitigationActionsTasksResponseTypeDef(TypedDict):
    tasks: List[DetectMitigationActionsTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DetectMitigationActionsTaskSummaryTypeDef](./type_defs.md#detectmitigationactionstasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThingTypesResponseTypeDef

```python
# ListThingTypesResponseTypeDef definition

class ListThingTypesResponseTypeDef(TypedDict):
    thingTypes: List[ThingTypeDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ThingTypeDefinitionTypeDef](./type_defs.md#thingtypedefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThingTypeRequestRequestTypeDef

```python
# CreateThingTypeRequestRequestTypeDef definition

class CreateThingTypeRequestRequestTypeDef(TypedDict):
    thingTypeName: str,
    thingTypeProperties: NotRequired[ThingTypePropertiesTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ThingTypePropertiesTypeDef](./type_defs.md#thingtypepropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateThingTypeRequestRequestTypeDef

```python
# UpdateThingTypeRequestRequestTypeDef definition

class UpdateThingTypeRequestRequestTypeDef(TypedDict):
    thingTypeName: str,
    thingTypeProperties: NotRequired[ThingTypePropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: ThingTypePropertiesTypeDef](./type_defs.md#thingtypepropertiestypedef) 
## DescribeAuditFindingResponseTypeDef

```python
# DescribeAuditFindingResponseTypeDef definition

class DescribeAuditFindingResponseTypeDef(TypedDict):
    finding: AuditFindingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuditFindingTypeDef](./type_defs.md#auditfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAuditFindingsResponseTypeDef

```python
# ListAuditFindingsResponseTypeDef definition

class ListAuditFindingsResponseTypeDef(TypedDict):
    findings: List[AuditFindingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditFindingTypeDef](./type_defs.md#auditfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TopicRuleTypeDef

```python
# TopicRuleTypeDef definition

class TopicRuleTypeDef(TypedDict):
    ruleName: NotRequired[str],
    sql: NotRequired[str],
    description: NotRequired[str],
    createdAt: NotRequired[datetime],
    actions: NotRequired[List[ActionOutputTypeDef]],  # (1)
    ruleDisabled: NotRequired[bool],
    awsIotSqlVersion: NotRequired[str],
    errorAction: NotRequired[ActionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
## CodeSigningTypeDef

```python
# CodeSigningTypeDef definition

class CodeSigningTypeDef(TypedDict):
    awsSignerJobId: NotRequired[str],
    startSigningJobParameter: NotRequired[StartSigningJobParameterTypeDef],  # (1)
    customCodeSigning: NotRequired[CustomCodeSigningUnionTypeDef],  # (2)
```

1. See [:material-code-braces: StartSigningJobParameterTypeDef](./type_defs.md#startsigningjobparametertypedef) 
2. See [:material-code-braces: CustomCodeSigningTypeDef](./type_defs.md#customcodesigningtypedef) [:material-code-braces: CustomCodeSigningOutputTypeDef](./type_defs.md#customcodesigningoutputtypedef) 
## CreateCommandRequestRequestTypeDef

```python
# CreateCommandRequestRequestTypeDef definition

class CreateCommandRequestRequestTypeDef(TypedDict):
    commandId: str,
    namespace: NotRequired[CommandNamespaceType],  # (1)
    displayName: NotRequired[str],
    description: NotRequired[str],
    payload: NotRequired[CommandPayloadTypeDef],  # (2)
    mandatoryParameters: NotRequired[Sequence[CommandParameterUnionTypeDef]],  # (3)
    roleArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-braces: CommandPayloadTypeDef](./type_defs.md#commandpayloadtypedef) 
3. See [:material-code-braces: CommandParameterTypeDef](./type_defs.md#commandparametertypedef) [:material-code-braces: CommandParameterOutputTypeDef](./type_defs.md#commandparameteroutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## OTAUpdateInfoTypeDef

```python
# OTAUpdateInfoTypeDef definition

class OTAUpdateInfoTypeDef(TypedDict):
    otaUpdateId: NotRequired[str],
    otaUpdateArn: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
    description: NotRequired[str],
    targets: NotRequired[List[str]],
    protocols: NotRequired[List[ProtocolType]],  # (1)
    awsJobExecutionsRolloutConfig: NotRequired[AwsJobExecutionsRolloutConfigTypeDef],  # (2)
    awsJobPresignedUrlConfig: NotRequired[AwsJobPresignedUrlConfigTypeDef],  # (3)
    targetSelection: NotRequired[TargetSelectionType],  # (4)
    otaUpdateFiles: NotRequired[List[OTAUpdateFileOutputTypeDef]],  # (5)
    otaUpdateStatus: NotRequired[OTAUpdateStatusType],  # (6)
    awsIotJobId: NotRequired[str],
    awsIotJobArn: NotRequired[str],
    errorInfo: NotRequired[ErrorInfoTypeDef],  # (7)
    additionalParameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-braces: AwsJobExecutionsRolloutConfigTypeDef](./type_defs.md#awsjobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AwsJobPresignedUrlConfigTypeDef](./type_defs.md#awsjobpresignedurlconfigtypedef) 
4. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
5. See [:material-code-braces: OTAUpdateFileOutputTypeDef](./type_defs.md#otaupdatefileoutputtypedef) 
6. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
7. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
## UpdateSecurityProfileRequestRequestTypeDef

```python
# UpdateSecurityProfileRequestRequestTypeDef definition

class UpdateSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileDescription: NotRequired[str],
    behaviors: NotRequired[Sequence[BehaviorTypeDef]],  # (1)
    alertTargets: NotRequired[Mapping[AlertTargetTypeType, AlertTargetTypeDef]],  # (2)
    additionalMetricsToRetain: NotRequired[Sequence[str]],
    additionalMetricsToRetainV2: NotRequired[Sequence[MetricToRetainTypeDef]],  # (3)
    deleteBehaviors: NotRequired[bool],
    deleteAlertTargets: NotRequired[bool],
    deleteAdditionalMetricsToRetain: NotRequired[bool],
    expectedVersion: NotRequired[int],
    metricsExportConfig: NotRequired[MetricsExportConfigTypeDef],  # (4)
    deleteMetricsExportConfig: NotRequired[bool],
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
## ValidateSecurityProfileBehaviorsRequestRequestTypeDef

```python
# ValidateSecurityProfileBehaviorsRequestRequestTypeDef definition

class ValidateSecurityProfileBehaviorsRequestRequestTypeDef(TypedDict):
    behaviors: Sequence[BehaviorTypeDef],  # (1)
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) 
## GetTopicRuleResponseTypeDef

```python
# GetTopicRuleResponseTypeDef definition

class GetTopicRuleResponseTypeDef(TypedDict):
    ruleArn: str,
    rule: TopicRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicRuleTypeDef](./type_defs.md#topicruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    dynamoDB: NotRequired[DynamoDBActionTypeDef],  # (1)
    dynamoDBv2: NotRequired[DynamoDBv2ActionTypeDef],  # (2)
    lambda: NotRequired[LambdaActionTypeDef],  # (3)
    sns: NotRequired[SnsActionTypeDef],  # (4)
    sqs: NotRequired[SqsActionTypeDef],  # (5)
    kinesis: NotRequired[KinesisActionTypeDef],  # (6)
    republish: NotRequired[RepublishActionUnionTypeDef],  # (7)
    s3: NotRequired[S3ActionTypeDef],  # (8)
    firehose: NotRequired[FirehoseActionTypeDef],  # (9)
    cloudwatchMetric: NotRequired[CloudwatchMetricActionTypeDef],  # (10)
    cloudwatchAlarm: NotRequired[CloudwatchAlarmActionTypeDef],  # (11)
    cloudwatchLogs: NotRequired[CloudwatchLogsActionTypeDef],  # (12)
    elasticsearch: NotRequired[ElasticsearchActionTypeDef],  # (13)
    salesforce: NotRequired[SalesforceActionTypeDef],  # (14)
    iotAnalytics: NotRequired[IotAnalyticsActionTypeDef],  # (15)
    iotEvents: NotRequired[IotEventsActionTypeDef],  # (16)
    iotSiteWise: NotRequired[IotSiteWiseActionUnionTypeDef],  # (17)
    stepFunctions: NotRequired[StepFunctionsActionTypeDef],  # (18)
    timestream: NotRequired[TimestreamActionUnionTypeDef],  # (19)
    http: NotRequired[HttpActionUnionTypeDef],  # (20)
    kafka: NotRequired[KafkaActionUnionTypeDef],  # (21)
    openSearch: NotRequired[OpenSearchActionTypeDef],  # (22)
    location: NotRequired[LocationActionTypeDef],  # (23)
```

1. See [:material-code-braces: DynamoDBActionTypeDef](./type_defs.md#dynamodbactiontypedef) 
2. See [:material-code-braces: DynamoDBv2ActionTypeDef](./type_defs.md#dynamodbv2actiontypedef) 
3. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
4. See [:material-code-braces: SnsActionTypeDef](./type_defs.md#snsactiontypedef) 
5. See [:material-code-braces: SqsActionTypeDef](./type_defs.md#sqsactiontypedef) 
6. See [:material-code-braces: KinesisActionTypeDef](./type_defs.md#kinesisactiontypedef) 
7. See [:material-code-braces: RepublishActionTypeDef](./type_defs.md#republishactiontypedef) [:material-code-braces: RepublishActionOutputTypeDef](./type_defs.md#republishactionoutputtypedef) 
8. See [:material-code-braces: S3ActionTypeDef](./type_defs.md#s3actiontypedef) 
9. See [:material-code-braces: FirehoseActionTypeDef](./type_defs.md#firehoseactiontypedef) 
10. See [:material-code-braces: CloudwatchMetricActionTypeDef](./type_defs.md#cloudwatchmetricactiontypedef) 
11. See [:material-code-braces: CloudwatchAlarmActionTypeDef](./type_defs.md#cloudwatchalarmactiontypedef) 
12. See [:material-code-braces: CloudwatchLogsActionTypeDef](./type_defs.md#cloudwatchlogsactiontypedef) 
13. See [:material-code-braces: ElasticsearchActionTypeDef](./type_defs.md#elasticsearchactiontypedef) 
14. See [:material-code-braces: SalesforceActionTypeDef](./type_defs.md#salesforceactiontypedef) 
15. See [:material-code-braces: IotAnalyticsActionTypeDef](./type_defs.md#iotanalyticsactiontypedef) 
16. See [:material-code-braces: IotEventsActionTypeDef](./type_defs.md#ioteventsactiontypedef) 
17. See [:material-code-braces: IotSiteWiseActionTypeDef](./type_defs.md#iotsitewiseactiontypedef) [:material-code-braces: IotSiteWiseActionOutputTypeDef](./type_defs.md#iotsitewiseactionoutputtypedef) 
18. See [:material-code-braces: StepFunctionsActionTypeDef](./type_defs.md#stepfunctionsactiontypedef) 
19. See [:material-code-braces: TimestreamActionTypeDef](./type_defs.md#timestreamactiontypedef) [:material-code-braces: TimestreamActionOutputTypeDef](./type_defs.md#timestreamactionoutputtypedef) 
20. See [:material-code-braces: HttpActionTypeDef](./type_defs.md#httpactiontypedef) [:material-code-braces: HttpActionOutputTypeDef](./type_defs.md#httpactionoutputtypedef) 
21. See [:material-code-braces: KafkaActionTypeDef](./type_defs.md#kafkaactiontypedef) [:material-code-braces: KafkaActionOutputTypeDef](./type_defs.md#kafkaactionoutputtypedef) 
22. See [:material-code-braces: OpenSearchActionTypeDef](./type_defs.md#opensearchactiontypedef) 
23. See [:material-code-braces: LocationActionTypeDef](./type_defs.md#locationactiontypedef) 
## GetOTAUpdateResponseTypeDef

```python
# GetOTAUpdateResponseTypeDef definition

class GetOTAUpdateResponseTypeDef(TypedDict):
    otaUpdateInfo: OTAUpdateInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OTAUpdateInfoTypeDef](./type_defs.md#otaupdateinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityProfileRequestRequestTypeDef

```python
# CreateSecurityProfileRequestRequestTypeDef definition

class CreateSecurityProfileRequestRequestTypeDef(TypedDict):
    securityProfileName: str,
    securityProfileDescription: NotRequired[str],
    behaviors: NotRequired[Sequence[BehaviorUnionTypeDef]],  # (1)
    alertTargets: NotRequired[Mapping[AlertTargetTypeType, AlertTargetTypeDef]],  # (2)
    additionalMetricsToRetain: NotRequired[Sequence[str]],
    additionalMetricsToRetainV2: NotRequired[Sequence[MetricToRetainTypeDef]],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    metricsExportConfig: NotRequired[MetricsExportConfigTypeDef],  # (5)
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
## OTAUpdateFileTypeDef

```python
# OTAUpdateFileTypeDef definition

class OTAUpdateFileTypeDef(TypedDict):
    fileName: NotRequired[str],
    fileType: NotRequired[int],
    fileVersion: NotRequired[str],
    fileLocation: NotRequired[FileLocationTypeDef],  # (1)
    codeSigning: NotRequired[CodeSigningUnionTypeDef],  # (2)
    attributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FileLocationTypeDef](./type_defs.md#filelocationtypedef) 
2. See [:material-code-braces: CodeSigningTypeDef](./type_defs.md#codesigningtypedef) [:material-code-braces: CodeSigningOutputTypeDef](./type_defs.md#codesigningoutputtypedef) 
## TopicRulePayloadTypeDef

```python
# TopicRulePayloadTypeDef definition

class TopicRulePayloadTypeDef(TypedDict):
    sql: str,
    actions: Sequence[ActionUnionTypeDef],  # (1)
    description: NotRequired[str],
    ruleDisabled: NotRequired[bool],
    awsIotSqlVersion: NotRequired[str],
    errorAction: NotRequired[ActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
## CreateTopicRuleRequestRequestTypeDef

```python
# CreateTopicRuleRequestRequestTypeDef definition

class CreateTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
    topicRulePayload: TopicRulePayloadTypeDef,  # (1)
    tags: NotRequired[str],
```

1. See [:material-code-braces: TopicRulePayloadTypeDef](./type_defs.md#topicrulepayloadtypedef) 
## ReplaceTopicRuleRequestRequestTypeDef

```python
# ReplaceTopicRuleRequestRequestTypeDef definition

class ReplaceTopicRuleRequestRequestTypeDef(TypedDict):
    ruleName: str,
    topicRulePayload: TopicRulePayloadTypeDef,  # (1)
```

1. See [:material-code-braces: TopicRulePayloadTypeDef](./type_defs.md#topicrulepayloadtypedef) 
## CreateOTAUpdateRequestRequestTypeDef

```python
# CreateOTAUpdateRequestRequestTypeDef definition

class CreateOTAUpdateRequestRequestTypeDef(TypedDict):
    otaUpdateId: str,
    targets: Sequence[str],
    files: Sequence[OTAUpdateFileUnionTypeDef],  # (1)
    roleArn: str,
    description: NotRequired[str],
    protocols: NotRequired[Sequence[ProtocolType]],  # (2)
    targetSelection: NotRequired[TargetSelectionType],  # (3)
    awsJobExecutionsRolloutConfig: NotRequired[AwsJobExecutionsRolloutConfigTypeDef],  # (4)
    awsJobPresignedUrlConfig: NotRequired[AwsJobPresignedUrlConfigTypeDef],  # (5)
    awsJobAbortConfig: NotRequired[AwsJobAbortConfigTypeDef],  # (6)
    awsJobTimeoutConfig: NotRequired[AwsJobTimeoutConfigTypeDef],  # (7)
    additionalParameters: NotRequired[Mapping[str, str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: OTAUpdateFileTypeDef](./type_defs.md#otaupdatefiletypedef) [:material-code-braces: OTAUpdateFileOutputTypeDef](./type_defs.md#otaupdatefileoutputtypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
4. See [:material-code-braces: AwsJobExecutionsRolloutConfigTypeDef](./type_defs.md#awsjobexecutionsrolloutconfigtypedef) 
5. See [:material-code-braces: AwsJobPresignedUrlConfigTypeDef](./type_defs.md#awsjobpresignedurlconfigtypedef) 
6. See [:material-code-braces: AwsJobAbortConfigTypeDef](./type_defs.md#awsjobabortconfigtypedef) 
7. See [:material-code-braces: AwsJobTimeoutConfigTypeDef](./type_defs.md#awsjobtimeoutconfigtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
