# Type definitions

> [Index](../README.md) > [QBusiness](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

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


## ActionExecutionPayloadFieldUnionTypeDef

```python
# ActionExecutionPayloadFieldUnionTypeDef definition

ActionExecutionPayloadFieldUnionTypeDef = Union[
    ActionExecutionPayloadFieldTypeDef,  # (1)
    ActionExecutionPayloadFieldOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionExecutionPayloadFieldTypeDef](./type_defs.md#actionexecutionpayloadfieldtypedef) 
2. See [:material-code-braces: ActionExecutionPayloadFieldOutputTypeDef](./type_defs.md#actionexecutionpayloadfieldoutputtypedef) 

## StringAttributeBoostingConfigurationUnionTypeDef

```python
# StringAttributeBoostingConfigurationUnionTypeDef definition

StringAttributeBoostingConfigurationUnionTypeDef = Union[
    StringAttributeBoostingConfigurationTypeDef,  # (1)
    StringAttributeBoostingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StringAttributeBoostingConfigurationTypeDef](./type_defs.md#stringattributeboostingconfigurationtypedef) 
2. See [:material-code-braces: StringAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#stringattributeboostingconfigurationoutputtypedef) 

## UsersAndGroupsUnionTypeDef

```python
# UsersAndGroupsUnionTypeDef definition

UsersAndGroupsUnionTypeDef = Union[
    UsersAndGroupsTypeDef,  # (1)
    UsersAndGroupsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef) 
2. See [:material-code-braces: UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef) 

## ContentRetrievalRuleUnionTypeDef

```python
# ContentRetrievalRuleUnionTypeDef definition

ContentRetrievalRuleUnionTypeDef = Union[
    ContentRetrievalRuleTypeDef,  # (1)
    ContentRetrievalRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef) 
2. See [:material-code-braces: ContentRetrievalRuleOutputTypeDef](./type_defs.md#contentretrievalruleoutputtypedef) 

## DocumentAttributeValueUnionTypeDef

```python
# DocumentAttributeValueUnionTypeDef definition

DocumentAttributeValueUnionTypeDef = Union[
    DocumentAttributeValueTypeDef,  # (1)
    DocumentAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
2. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 

## DocumentAttributeBoostingConfigurationUnionTypeDef

```python
# DocumentAttributeBoostingConfigurationUnionTypeDef definition

DocumentAttributeBoostingConfigurationUnionTypeDef = Union[
    DocumentAttributeBoostingConfigurationTypeDef,  # (1)
    DocumentAttributeBoostingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeBoostingConfigurationTypeDef](./type_defs.md#documentattributeboostingconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#documentattributeboostingconfigurationoutputtypedef) 

## RuleConfigurationUnionTypeDef

```python
# RuleConfigurationUnionTypeDef definition

RuleConfigurationUnionTypeDef = Union[
    RuleConfigurationTypeDef,  # (1)
    RuleConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef) 
2. See [:material-code-braces: RuleConfigurationOutputTypeDef](./type_defs.md#ruleconfigurationoutputtypedef) 

## DocumentAttributeConditionUnionTypeDef

```python
# DocumentAttributeConditionUnionTypeDef definition

DocumentAttributeConditionUnionTypeDef = Union[
    DocumentAttributeConditionTypeDef,  # (1)
    DocumentAttributeConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) 
2. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 

## DocumentAttributeTargetUnionTypeDef

```python
# DocumentAttributeTargetUnionTypeDef definition

DocumentAttributeTargetUnionTypeDef = Union[
    DocumentAttributeTargetTypeDef,  # (1)
    DocumentAttributeTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef) 
2. See [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 

## NativeIndexConfigurationUnionTypeDef

```python
# NativeIndexConfigurationUnionTypeDef definition

NativeIndexConfigurationUnionTypeDef = Union[
    NativeIndexConfigurationTypeDef,  # (1)
    NativeIndexConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef) 
2. See [:material-code-braces: NativeIndexConfigurationOutputTypeDef](./type_defs.md#nativeindexconfigurationoutputtypedef) 

## RuleUnionTypeDef

```python
# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 

## HookConfigurationUnionTypeDef

```python
# HookConfigurationUnionTypeDef definition

HookConfigurationUnionTypeDef = Union[
    HookConfigurationTypeDef,  # (1)
    HookConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) 
2. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 

## InlineDocumentEnrichmentConfigurationUnionTypeDef

```python
# InlineDocumentEnrichmentConfigurationUnionTypeDef definition

InlineDocumentEnrichmentConfigurationUnionTypeDef = Union[
    InlineDocumentEnrichmentConfigurationTypeDef,  # (1)
    InlineDocumentEnrichmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: InlineDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationoutputtypedef) 

## TopicConfigurationUnionTypeDef

```python
# TopicConfigurationUnionTypeDef definition

TopicConfigurationUnionTypeDef = Union[
    TopicConfigurationTypeDef,  # (1)
    TopicConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
2. See [:material-code-braces: TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef) 

## DocumentEnrichmentConfigurationUnionTypeDef

```python
# DocumentEnrichmentConfigurationUnionTypeDef definition

DocumentEnrichmentConfigurationUnionTypeDef = Union[
    DocumentEnrichmentConfigurationTypeDef,  # (1)
    DocumentEnrichmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: DocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#documentenrichmentconfigurationoutputtypedef) 



## S3TypeDef

```python
# S3TypeDef definition

class S3TypeDef(TypedDict):
    bucket: str,
    key: str,
```

## ActionExecutionPayloadFieldOutputTypeDef

```python
# ActionExecutionPayloadFieldOutputTypeDef definition

class ActionExecutionPayloadFieldOutputTypeDef(TypedDict):
    value: Dict[str, Any],
```

## ActionExecutionPayloadFieldTypeDef

```python
# ActionExecutionPayloadFieldTypeDef definition

class ActionExecutionPayloadFieldTypeDef(TypedDict):
    value: Mapping[str, Any],
```

## ActionReviewPayloadFieldAllowedValueTypeDef

```python
# ActionReviewPayloadFieldAllowedValueTypeDef definition

class ActionReviewPayloadFieldAllowedValueTypeDef(TypedDict):
    value: NotRequired[Dict[str, Any]],
    displayValue: NotRequired[Dict[str, Any]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    displayName: NotRequired[str],
    applicationId: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    status: NotRequired[ApplicationStatusType],  # (1)
    identityType: NotRequired[IdentityTypeType],  # (2)
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
2. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## AppliedAttachmentsConfigurationTypeDef

```python
# AppliedAttachmentsConfigurationTypeDef definition

class AppliedAttachmentsConfigurationTypeDef(TypedDict):
    attachmentsControlMode: NotRequired[AttachmentsControlModeType],  # (1)
```

1. See [:material-code-brackets: AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype) 
## AppliedCreatorModeConfigurationTypeDef

```python
# AppliedCreatorModeConfigurationTypeDef definition

class AppliedCreatorModeConfigurationTypeDef(TypedDict):
    creatorModeControl: CreatorModeControlType,  # (1)
```

1. See [:material-code-brackets: CreatorModeControlType](./literals.md#creatormodecontroltype) 
## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## AttachmentsConfigurationTypeDef

```python
# AttachmentsConfigurationTypeDef definition

class AttachmentsConfigurationTypeDef(TypedDict):
    attachmentsControlMode: AttachmentsControlModeType,  # (1)
```

1. See [:material-code-brackets: AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype) 
## AuthChallengeRequestTypeDef

```python
# AuthChallengeRequestTypeDef definition

class AuthChallengeRequestTypeDef(TypedDict):
    authorizationUrl: str,
```

## AuthChallengeResponseTypeDef

```python
# AuthChallengeResponseTypeDef definition

class AuthChallengeResponseTypeDef(TypedDict):
    responseMap: Mapping[str, str],
```

## AutoSubscriptionConfigurationTypeDef

```python
# AutoSubscriptionConfigurationTypeDef definition

class AutoSubscriptionConfigurationTypeDef(TypedDict):
    autoSubscribe: AutoSubscriptionStatusType,  # (1)
    defaultSubscriptionType: NotRequired[SubscriptionTypeType],  # (2)
```

1. See [:material-code-brackets: AutoSubscriptionStatusType](./literals.md#autosubscriptionstatustype) 
2. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
## BasicAuthConfigurationTypeDef

```python
# BasicAuthConfigurationTypeDef definition

class BasicAuthConfigurationTypeDef(TypedDict):
    secretArn: str,
    roleArn: str,
```

## DeleteDocumentTypeDef

```python
# DeleteDocumentTypeDef definition

class DeleteDocumentTypeDef(TypedDict):
    documentId: str,
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

## BlockedPhrasesConfigurationTypeDef

```python
# BlockedPhrasesConfigurationTypeDef definition

class BlockedPhrasesConfigurationTypeDef(TypedDict):
    blockedPhrases: NotRequired[List[str]],
    systemMessageOverride: NotRequired[str],
```

## BlockedPhrasesConfigurationUpdateTypeDef

```python
# BlockedPhrasesConfigurationUpdateTypeDef definition

class BlockedPhrasesConfigurationUpdateTypeDef(TypedDict):
    blockedPhrasesToCreateOrUpdate: NotRequired[Sequence[str]],
    blockedPhrasesToDelete: NotRequired[Sequence[str]],
    systemMessageOverride: NotRequired[str],
```

## PluginConfigurationTypeDef

```python
# PluginConfigurationTypeDef definition

class PluginConfigurationTypeDef(TypedDict):
    pluginId: str,
```

## ContentBlockerRuleTypeDef

```python
# ContentBlockerRuleTypeDef definition

class ContentBlockerRuleTypeDef(TypedDict):
    systemMessageOverride: NotRequired[str],
```

## EligibleDataSourceTypeDef

```python
# EligibleDataSourceTypeDef definition

class EligibleDataSourceTypeDef(TypedDict):
    indexId: NotRequired[str],
    dataSourceId: NotRequired[str],
```

## ConversationTypeDef

```python
# ConversationTypeDef definition

class ConversationTypeDef(TypedDict):
    conversationId: NotRequired[str],
    title: NotRequired[str],
    startTime: NotRequired[datetime],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## PersonalizationConfigurationTypeDef

```python
# PersonalizationConfigurationTypeDef definition

class PersonalizationConfigurationTypeDef(TypedDict):
    personalizationControlMode: PersonalizationControlModeType,  # (1)
```

1. See [:material-code-brackets: PersonalizationControlModeType](./literals.md#personalizationcontrolmodetype) 
## QAppsConfigurationTypeDef

```python
# QAppsConfigurationTypeDef definition

class QAppsConfigurationTypeDef(TypedDict):
    qAppsControlMode: QAppsControlModeType,  # (1)
```

1. See [:material-code-brackets: QAppsControlModeType](./literals.md#qappscontrolmodetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## DataSourceVpcConfigurationTypeDef

```python
# DataSourceVpcConfigurationTypeDef definition

class DataSourceVpcConfigurationTypeDef(TypedDict):
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
```

## IndexCapacityConfigurationTypeDef

```python
# IndexCapacityConfigurationTypeDef definition

class IndexCapacityConfigurationTypeDef(TypedDict):
    units: NotRequired[int],
```

## UserAliasTypeDef

```python
# UserAliasTypeDef definition

class UserAliasTypeDef(TypedDict):
    userId: str,
    indexId: NotRequired[str],
    dataSourceId: NotRequired[str],
```

## CreatorModeConfigurationTypeDef

```python
# CreatorModeConfigurationTypeDef definition

class CreatorModeConfigurationTypeDef(TypedDict):
    creatorModeControl: CreatorModeControlType,  # (1)
```

1. See [:material-code-brackets: CreatorModeControlType](./literals.md#creatormodecontroltype) 
## DataSourceSyncJobMetricsTypeDef

```python
# DataSourceSyncJobMetricsTypeDef definition

class DataSourceSyncJobMetricsTypeDef(TypedDict):
    documentsAdded: NotRequired[str],
    documentsModified: NotRequired[str],
    documentsDeleted: NotRequired[str],
    documentsFailed: NotRequired[str],
    documentsScanned: NotRequired[str],
```

## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    displayName: NotRequired[str],
    dataSourceId: NotRequired[str],
    type: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    status: NotRequired[DataSourceStatusType],  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## DataSourceVpcConfigurationOutputTypeDef

```python
# DataSourceVpcConfigurationOutputTypeDef definition

class DataSourceVpcConfigurationOutputTypeDef(TypedDict):
    subnetIds: List[str],
    securityGroupIds: List[str],
```

## DateAttributeBoostingConfigurationTypeDef

```python
# DateAttributeBoostingConfigurationTypeDef definition

class DateAttributeBoostingConfigurationTypeDef(TypedDict):
    boostingLevel: DocumentAttributeBoostingLevelType,  # (1)
    boostingDurationInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype) 
## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## DeleteChatControlsConfigurationRequestRequestTypeDef

```python
# DeleteChatControlsConfigurationRequestRequestTypeDef definition

class DeleteChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## DeleteConversationRequestRequestTypeDef

```python
# DeleteConversationRequestRequestTypeDef definition

class DeleteConversationRequestRequestTypeDef(TypedDict):
    conversationId: str,
    applicationId: str,
    userId: NotRequired[str],
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceId: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    groupName: str,
    dataSourceId: NotRequired[str],
```

## DeleteIndexRequestRequestTypeDef

```python
# DeleteIndexRequestRequestTypeDef definition

class DeleteIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
```

## DeletePluginRequestRequestTypeDef

```python
# DeletePluginRequestRequestTypeDef definition

class DeletePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
```

## DeleteRetrieverRequestRequestTypeDef

```python
# DeleteRetrieverRequestRequestTypeDef definition

class DeleteRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
```

## DeleteWebExperienceRequestRequestTypeDef

```python
# DeleteWebExperienceRequestRequestTypeDef definition

class DeleteWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
```

## NumberAttributeBoostingConfigurationTypeDef

```python
# NumberAttributeBoostingConfigurationTypeDef definition

class NumberAttributeBoostingConfigurationTypeDef(TypedDict):
    boostingLevel: DocumentAttributeBoostingLevelType,  # (1)
    boostingType: NotRequired[NumberAttributeBoostingTypeType],  # (2)
```

1. See [:material-code-brackets: DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype) 
2. See [:material-code-brackets: NumberAttributeBoostingTypeType](./literals.md#numberattributeboostingtypetype) 
## StringAttributeBoostingConfigurationOutputTypeDef

```python
# StringAttributeBoostingConfigurationOutputTypeDef definition

class StringAttributeBoostingConfigurationOutputTypeDef(TypedDict):
    boostingLevel: DocumentAttributeBoostingLevelType,  # (1)
    attributeValueBoosting: NotRequired[Dict[str, StringAttributeValueBoostingLevelType]],  # (2)
```

1. See [:material-code-brackets: DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype) 
2. See [:material-code-brackets: StringAttributeValueBoostingLevelType](./literals.md#stringattributevalueboostingleveltype) 
## StringListAttributeBoostingConfigurationTypeDef

```python
# StringListAttributeBoostingConfigurationTypeDef definition

class StringListAttributeBoostingConfigurationTypeDef(TypedDict):
    boostingLevel: DocumentAttributeBoostingLevelType,  # (1)
```

1. See [:material-code-brackets: DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype) 
## DocumentAttributeValueOutputTypeDef

```python
# DocumentAttributeValueOutputTypeDef definition

class DocumentAttributeValueOutputTypeDef(TypedDict):
    stringValue: NotRequired[str],
    stringListValue: NotRequired[List[str]],
    longValue: NotRequired[int],
    dateValue: NotRequired[datetime],
```

## DocumentAttributeConfigurationTypeDef

```python
# DocumentAttributeConfigurationTypeDef definition

class DocumentAttributeConfigurationTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[AttributeTypeType],  # (1)
    search: NotRequired[StatusType],  # (2)
```

1. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetChatControlsConfigurationRequestRequestTypeDef

```python
# GetChatControlsConfigurationRequestRequestTypeDef definition

class GetChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetDataSourceRequestRequestTypeDef

```python
# GetDataSourceRequestRequestTypeDef definition

class GetDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceId: str,
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    groupName: str,
    dataSourceId: NotRequired[str],
```

## GetIndexRequestRequestTypeDef

```python
# GetIndexRequestRequestTypeDef definition

class GetIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
```

## GetPluginRequestRequestTypeDef

```python
# GetPluginRequestRequestTypeDef definition

class GetPluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
```

## GetRetrieverRequestRequestTypeDef

```python
# GetRetrieverRequestRequestTypeDef definition

class GetRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
```

## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
```

## GetWebExperienceRequestRequestTypeDef

```python
# GetWebExperienceRequestRequestTypeDef definition

class GetWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
```

## MemberGroupTypeDef

```python
# MemberGroupTypeDef definition

class MemberGroupTypeDef(TypedDict):
    groupName: str,
    type: NotRequired[MembershipTypeType],  # (1)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## MemberUserTypeDef

```python
# MemberUserTypeDef definition

class MemberUserTypeDef(TypedDict):
    userId: str,
    type: NotRequired[MembershipTypeType],  # (1)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## OpenIDConnectProviderConfigurationTypeDef

```python
# OpenIDConnectProviderConfigurationTypeDef definition

class OpenIDConnectProviderConfigurationTypeDef(TypedDict):
    secretsArn: str,
    secretsRole: str,
```

## SamlProviderConfigurationTypeDef

```python
# SamlProviderConfigurationTypeDef definition

class SamlProviderConfigurationTypeDef(TypedDict):
    authenticationUrl: str,
```

## TextDocumentStatisticsTypeDef

```python
# TextDocumentStatisticsTypeDef definition

class TextDocumentStatisticsTypeDef(TypedDict):
    indexedTextBytes: NotRequired[int],
    indexedTextDocumentCount: NotRequired[int],
```

## IndexTypeDef

```python
# IndexTypeDef definition

class IndexTypeDef(TypedDict):
    displayName: NotRequired[str],
    indexId: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    status: NotRequired[IndexStatusType],  # (1)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## KendraIndexConfigurationTypeDef

```python
# KendraIndexConfigurationTypeDef definition

class KendraIndexConfigurationTypeDef(TypedDict):
    indexId: str,
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConversationsRequestRequestTypeDef

```python
# ListConversationsRequestRequestTypeDef definition

class ListConversationsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDocumentsRequestRequestTypeDef

```python
# ListDocumentsRequestRequestTypeDef definition

class ListDocumentsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListIndicesRequestRequestTypeDef

```python
# ListIndicesRequestRequestTypeDef definition

class ListIndicesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMessagesRequestRequestTypeDef

```python
# ListMessagesRequestRequestTypeDef definition

class ListMessagesRequestRequestTypeDef(TypedDict):
    conversationId: str,
    applicationId: str,
    userId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPluginsRequestRequestTypeDef

```python
# ListPluginsRequestRequestTypeDef definition

class ListPluginsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PluginTypeDef

```python
# PluginTypeDef definition

class PluginTypeDef(TypedDict):
    pluginId: NotRequired[str],
    displayName: NotRequired[str],
    type: NotRequired[PluginTypeType],  # (1)
    serverUrl: NotRequired[str],
    state: NotRequired[PluginStateType],  # (2)
    buildStatus: NotRequired[PluginBuildStatusType],  # (3)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
3. See [:material-code-brackets: PluginBuildStatusType](./literals.md#pluginbuildstatustype) 
## ListRetrieversRequestRequestTypeDef

```python
# ListRetrieversRequestRequestTypeDef definition

class ListRetrieversRequestRequestTypeDef(TypedDict):
    applicationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RetrieverTypeDef

```python
# RetrieverTypeDef definition

class RetrieverTypeDef(TypedDict):
    applicationId: NotRequired[str],
    retrieverId: NotRequired[str],
    type: NotRequired[RetrieverTypeType],  # (1)
    status: NotRequired[RetrieverStatusType],  # (2)
    displayName: NotRequired[str],
```

1. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
2. See [:material-code-brackets: RetrieverStatusType](./literals.md#retrieverstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
```

## ListWebExperiencesRequestRequestTypeDef

```python
# ListWebExperiencesRequestRequestTypeDef definition

class ListWebExperiencesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## WebExperienceTypeDef

```python
# WebExperienceTypeDef definition

class WebExperienceTypeDef(TypedDict):
    webExperienceId: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    defaultEndpoint: NotRequired[str],
    status: NotRequired[WebExperienceStatusType],  # (1)
```

1. See [:material-code-brackets: WebExperienceStatusType](./literals.md#webexperiencestatustype) 
## OAuth2ClientCredentialConfigurationTypeDef

```python
# OAuth2ClientCredentialConfigurationTypeDef definition

class OAuth2ClientCredentialConfigurationTypeDef(TypedDict):
    secretArn: str,
    roleArn: str,
```

## PrincipalGroupTypeDef

```python
# PrincipalGroupTypeDef definition

class PrincipalGroupTypeDef(TypedDict):
    access: ReadAccessTypeType,  # (1)
    name: NotRequired[str],
    membershipType: NotRequired[MembershipTypeType],  # (2)
```

1. See [:material-code-brackets: ReadAccessTypeType](./literals.md#readaccesstypetype) 
2. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## PrincipalUserTypeDef

```python
# PrincipalUserTypeDef definition

class PrincipalUserTypeDef(TypedDict):
    access: ReadAccessTypeType,  # (1)
    id: NotRequired[str],
    membershipType: NotRequired[MembershipTypeType],  # (2)
```

1. See [:material-code-brackets: ReadAccessTypeType](./literals.md#readaccesstypetype) 
2. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## UsersAndGroupsOutputTypeDef

```python
# UsersAndGroupsOutputTypeDef definition

class UsersAndGroupsOutputTypeDef(TypedDict):
    userIds: NotRequired[List[str]],
    userGroups: NotRequired[List[str]],
```

## SamlConfigurationTypeDef

```python
# SamlConfigurationTypeDef definition

class SamlConfigurationTypeDef(TypedDict):
    metadataXML: str,
    roleArn: str,
    userIdAttribute: str,
    userGroupAttribute: NotRequired[str],
```

## SnippetExcerptTypeDef

```python
# SnippetExcerptTypeDef definition

class SnippetExcerptTypeDef(TypedDict):
    text: NotRequired[str],
```

## StartDataSourceSyncJobRequestRequestTypeDef

```python
# StartDataSourceSyncJobRequestRequestTypeDef definition

class StartDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    applicationId: str,
    indexId: str,
```

## StopDataSourceSyncJobRequestRequestTypeDef

```python
# StopDataSourceSyncJobRequestRequestTypeDef definition

class StopDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    applicationId: str,
    indexId: str,
```

## StringAttributeBoostingConfigurationTypeDef

```python
# StringAttributeBoostingConfigurationTypeDef definition

class StringAttributeBoostingConfigurationTypeDef(TypedDict):
    boostingLevel: DocumentAttributeBoostingLevelType,  # (1)
    attributeValueBoosting: NotRequired[Mapping[str, StringAttributeValueBoostingLevelType]],  # (2)
```

1. See [:material-code-brackets: DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype) 
2. See [:material-code-brackets: StringAttributeValueBoostingLevelType](./literals.md#stringattributevalueboostingleveltype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UsersAndGroupsTypeDef

```python
# UsersAndGroupsTypeDef definition

class UsersAndGroupsTypeDef(TypedDict):
    userIds: NotRequired[Sequence[str]],
    userGroups: NotRequired[Sequence[str]],
```

## APISchemaTypeDef

```python
# APISchemaTypeDef definition

class APISchemaTypeDef(TypedDict):
    payload: NotRequired[str],
    s3: NotRequired[S3TypeDef],  # (1)
```

1. See [:material-code-braces: S3TypeDef](./type_defs.md#s3typedef) 
## ActionExecutionOutputTypeDef

```python
# ActionExecutionOutputTypeDef definition

class ActionExecutionOutputTypeDef(TypedDict):
    pluginId: str,
    payload: Dict[str, ActionExecutionPayloadFieldOutputTypeDef],  # (1)
    payloadFieldNameSeparator: str,
```

1. See [:material-code-braces: ActionExecutionPayloadFieldOutputTypeDef](./type_defs.md#actionexecutionpayloadfieldoutputtypedef) 
## ActionReviewPayloadFieldTypeDef

```python
# ActionReviewPayloadFieldTypeDef definition

class ActionReviewPayloadFieldTypeDef(TypedDict):
    displayName: NotRequired[str],
    displayOrder: NotRequired[int],
    displayDescription: NotRequired[str],
    type: NotRequired[ActionPayloadFieldTypeType],  # (1)
    value: NotRequired[Dict[str, Any]],
    allowedValues: NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],  # (2)
    allowedFormat: NotRequired[str],
    arrayItemJsonSchema: NotRequired[Dict[str, Any]],
    required: NotRequired[bool],
```

1. See [:material-code-brackets: ActionPayloadFieldTypeType](./literals.md#actionpayloadfieldtypetype) 
2. See [:material-code-braces: ActionReviewPayloadFieldAllowedValueTypeDef](./type_defs.md#actionreviewpayloadfieldallowedvaluetypedef) 
## AttachmentInputTypeDef

```python
# AttachmentInputTypeDef definition

class AttachmentInputTypeDef(TypedDict):
    name: str,
    data: BlobTypeDef,
```

## DocumentContentTypeDef

```python
# DocumentContentTypeDef definition

class DocumentContentTypeDef(TypedDict):
    blob: NotRequired[BlobTypeDef],
    s3: NotRequired[S3TypeDef],  # (1)
```

1. See [:material-code-braces: S3TypeDef](./type_defs.md#s3typedef) 
## AttachmentOutputTypeDef

```python
# AttachmentOutputTypeDef definition

class AttachmentOutputTypeDef(TypedDict):
    name: NotRequired[str],
    status: NotRequired[AttachmentStatusType],  # (1)
    error: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## DocumentDetailsTypeDef

```python
# DocumentDetailsTypeDef definition

class DocumentDetailsTypeDef(TypedDict):
    documentId: NotRequired[str],
    status: NotRequired[DocumentStatusType],  # (1)
    error: NotRequired[ErrorDetailTypeDef],  # (2)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## FailedDocumentTypeDef

```python
# FailedDocumentTypeDef definition

class FailedDocumentTypeDef(TypedDict):
    id: NotRequired[str],
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    dataSourceId: NotRequired[str],
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## GroupStatusDetailTypeDef

```python
# GroupStatusDetailTypeDef definition

class GroupStatusDetailTypeDef(TypedDict):
    status: NotRequired[GroupStatusType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    errorDetail: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-brackets: GroupStatusType](./literals.md#groupstatustype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## BatchDeleteDocumentRequestRequestTypeDef

```python
# BatchDeleteDocumentRequestRequestTypeDef definition

class BatchDeleteDocumentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    documents: Sequence[DeleteDocumentTypeDef],  # (1)
    dataSourceSyncId: NotRequired[str],
```

1. See [:material-code-braces: DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    applicationId: str,
    applicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    dataSourceId: str,
    dataSourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexResponseTypeDef

```python
# CreateIndexResponseTypeDef definition

class CreateIndexResponseTypeDef(TypedDict):
    indexId: str,
    indexArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePluginResponseTypeDef

```python
# CreatePluginResponseTypeDef definition

class CreatePluginResponseTypeDef(TypedDict):
    pluginId: str,
    pluginArn: str,
    buildStatus: PluginBuildStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PluginBuildStatusType](./literals.md#pluginbuildstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRetrieverResponseTypeDef

```python
# CreateRetrieverResponseTypeDef definition

class CreateRetrieverResponseTypeDef(TypedDict):
    retrieverId: str,
    retrieverArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWebExperienceResponseTypeDef

```python
# CreateWebExperienceResponseTypeDef definition

class CreateWebExperienceResponseTypeDef(TypedDict):
    webExperienceId: str,
    webExperienceArn: str,
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
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    applications: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataSourceSyncJobResponseTypeDef

```python
# StartDataSourceSyncJobResponseTypeDef definition

class StartDataSourceSyncJobResponseTypeDef(TypedDict):
    executionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChatModeConfigurationTypeDef

```python
# ChatModeConfigurationTypeDef definition

class ChatModeConfigurationTypeDef(TypedDict):
    pluginConfiguration: NotRequired[PluginConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PluginConfigurationTypeDef](./type_defs.md#pluginconfigurationtypedef) 
## ContentRetrievalRuleOutputTypeDef

```python
# ContentRetrievalRuleOutputTypeDef definition

class ContentRetrievalRuleOutputTypeDef(TypedDict):
    eligibleDataSources: NotRequired[List[EligibleDataSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef) 
## ContentRetrievalRuleTypeDef

```python
# ContentRetrievalRuleTypeDef definition

class ContentRetrievalRuleTypeDef(TypedDict):
    eligibleDataSources: NotRequired[Sequence[EligibleDataSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef) 
## ListConversationsResponseTypeDef

```python
# ListConversationsResponseTypeDef definition

class ListConversationsResponseTypeDef(TypedDict):
    conversations: List[ConversationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConversationTypeDef](./type_defs.md#conversationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    displayName: str,
    applicationId: str,
    applicationArn: str,
    identityType: IdentityTypeType,  # (1)
    iamIdentityProviderArn: str,
    identityCenterApplicationArn: str,
    roleArn: str,
    status: ApplicationStatusType,  # (2)
    description: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef,  # (3)
    createdAt: datetime,
    updatedAt: datetime,
    error: ErrorDetailTypeDef,  # (4)
    attachmentsConfiguration: AppliedAttachmentsConfigurationTypeDef,  # (5)
    qAppsConfiguration: QAppsConfigurationTypeDef,  # (6)
    personalizationConfiguration: PersonalizationConfigurationTypeDef,  # (7)
    autoSubscriptionConfiguration: AutoSubscriptionConfigurationTypeDef,  # (8)
    clientIdsForOIDC: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
5. See [:material-code-braces: AppliedAttachmentsConfigurationTypeDef](./type_defs.md#appliedattachmentsconfigurationtypedef) 
6. See [:material-code-braces: QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef) 
7. See [:material-code-braces: PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef) 
8. See [:material-code-braces: AutoSubscriptionConfigurationTypeDef](./type_defs.md#autosubscriptionconfigurationtypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    identityCenterInstanceArn: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    roleArn: NotRequired[str],
    attachmentsConfiguration: NotRequired[AttachmentsConfigurationTypeDef],  # (1)
    qAppsConfiguration: NotRequired[QAppsConfigurationTypeDef],  # (2)
    personalizationConfiguration: NotRequired[PersonalizationConfigurationTypeDef],  # (3)
    autoSubscriptionConfiguration: NotRequired[AutoSubscriptionConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
2. See [:material-code-braces: QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef) 
3. See [:material-code-braces: PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef) 
4. See [:material-code-braces: AutoSubscriptionConfigurationTypeDef](./type_defs.md#autosubscriptionconfigurationtypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    displayName: str,
    roleArn: NotRequired[str],
    identityType: NotRequired[IdentityTypeType],  # (1)
    iamIdentityProviderArn: NotRequired[str],
    identityCenterInstanceArn: NotRequired[str],
    clientIdsForOIDC: NotRequired[Sequence[str]],
    description: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    clientToken: NotRequired[str],
    attachmentsConfiguration: NotRequired[AttachmentsConfigurationTypeDef],  # (4)
    qAppsConfiguration: NotRequired[QAppsConfigurationTypeDef],  # (5)
    personalizationConfiguration: NotRequired[PersonalizationConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
5. See [:material-code-braces: QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef) 
6. See [:material-code-braces: PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIndexRequestRequestTypeDef

```python
# CreateIndexRequestRequestTypeDef definition

class CreateIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    displayName: str,
    type: NotRequired[IndexTypeType],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    capacityConfiguration: NotRequired[IndexCapacityConfigurationTypeDef],  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    userAliases: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    userAliases: List[UserAliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    userAliasesToUpdate: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
    userAliasesToDelete: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    userAliasesAdded: List[UserAliasTypeDef],  # (1)
    userAliasesUpdated: List[UserAliasTypeDef],  # (1)
    userAliasesDeleted: List[UserAliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
3. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceSyncJobTypeDef

```python
# DataSourceSyncJobTypeDef definition

class DataSourceSyncJobTypeDef(TypedDict):
    executionId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    status: NotRequired[DataSourceSyncJobStatusType],  # (1)
    error: NotRequired[ErrorDetailTypeDef],  # (2)
    dataSourceErrorCode: NotRequired[str],
    metrics: NotRequired[DataSourceSyncJobMetricsTypeDef],  # (3)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
3. See [:material-code-braces: DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    dataSources: List[DataSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentAttributeBoostingConfigurationOutputTypeDef

```python
# DocumentAttributeBoostingConfigurationOutputTypeDef definition

class DocumentAttributeBoostingConfigurationOutputTypeDef(TypedDict):
    numberConfiguration: NotRequired[NumberAttributeBoostingConfigurationTypeDef],  # (1)
    stringConfiguration: NotRequired[StringAttributeBoostingConfigurationOutputTypeDef],  # (2)
    dateConfiguration: NotRequired[DateAttributeBoostingConfigurationTypeDef],  # (3)
    stringListConfiguration: NotRequired[StringListAttributeBoostingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: NumberAttributeBoostingConfigurationTypeDef](./type_defs.md#numberattributeboostingconfigurationtypedef) 
2. See [:material-code-braces: StringAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#stringattributeboostingconfigurationoutputtypedef) 
3. See [:material-code-braces: DateAttributeBoostingConfigurationTypeDef](./type_defs.md#dateattributeboostingconfigurationtypedef) 
4. See [:material-code-braces: StringListAttributeBoostingConfigurationTypeDef](./type_defs.md#stringlistattributeboostingconfigurationtypedef) 
## DocumentAttributeConditionOutputTypeDef

```python
# DocumentAttributeConditionOutputTypeDef definition

class DocumentAttributeConditionOutputTypeDef(TypedDict):
    key: str,
    operator: DocumentEnrichmentConditionOperatorType,  # (1)
    value: NotRequired[DocumentAttributeValueOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: DocumentEnrichmentConditionOperatorType](./literals.md#documentenrichmentconditionoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeTargetOutputTypeDef

```python
# DocumentAttributeTargetOutputTypeDef definition

class DocumentAttributeTargetOutputTypeDef(TypedDict):
    key: str,
    value: NotRequired[DocumentAttributeValueOutputTypeDef],  # (1)
    attributeValueOperator: NotRequired[AttributeValueOperatorType],  # (2)
```

1. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
2. See [:material-code-brackets: AttributeValueOperatorType](./literals.md#attributevalueoperatortype) 
## UpdateIndexRequestRequestTypeDef

```python
# UpdateIndexRequestRequestTypeDef definition

class UpdateIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
    capacityConfiguration: NotRequired[IndexCapacityConfigurationTypeDef],  # (1)
    documentAttributeConfigurations: NotRequired[Sequence[DocumentAttributeConfigurationTypeDef]],  # (2)
```

1. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef) 
## DocumentAttributeValueTypeDef

```python
# DocumentAttributeValueTypeDef definition

class DocumentAttributeValueTypeDef(TypedDict):
    stringValue: NotRequired[str],
    stringListValue: NotRequired[Sequence[str]],
    longValue: NotRequired[int],
    dateValue: NotRequired[TimestampTypeDef],
```

## ListDataSourceSyncJobsRequestRequestTypeDef

```python
# ListDataSourceSyncJobsRequestRequestTypeDef definition

class ListDataSourceSyncJobsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    applicationId: str,
    indexId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    statusFilter: NotRequired[DataSourceSyncJobStatusType],  # (1)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    updatedEarlierThan: TimestampTypeDef,
    dataSourceId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MessageUsefulnessFeedbackTypeDef

```python
# MessageUsefulnessFeedbackTypeDef definition

class MessageUsefulnessFeedbackTypeDef(TypedDict):
    usefulness: MessageUsefulnessType,  # (1)
    submittedAt: TimestampTypeDef,
    reason: NotRequired[MessageUsefulnessReasonType],  # (2)
    comment: NotRequired[str],
```

1. See [:material-code-brackets: MessageUsefulnessType](./literals.md#messageusefulnesstype) 
2. See [:material-code-brackets: MessageUsefulnessReasonType](./literals.md#messageusefulnessreasontype) 
## GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef

```python
# GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef definition

class GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConversationsRequestListConversationsPaginateTypeDef

```python
# ListConversationsRequestListConversationsPaginateTypeDef definition

class ListConversationsRequestListConversationsPaginateTypeDef(TypedDict):
    applicationId: str,
    userId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef

```python
# ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef definition

class ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef(TypedDict):
    dataSourceId: str,
    applicationId: str,
    indexId: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    statusFilter: NotRequired[DataSourceSyncJobStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesRequestListDataSourcesPaginateTypeDef

```python
# ListDataSourcesRequestListDataSourcesPaginateTypeDef definition

class ListDataSourcesRequestListDataSourcesPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentsRequestListDocumentsPaginateTypeDef

```python
# ListDocumentsRequestListDocumentsPaginateTypeDef definition

class ListDocumentsRequestListDocumentsPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestListGroupsPaginateTypeDef

```python
# ListGroupsRequestListGroupsPaginateTypeDef definition

class ListGroupsRequestListGroupsPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    updatedEarlierThan: TimestampTypeDef,
    dataSourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndicesRequestListIndicesPaginateTypeDef

```python
# ListIndicesRequestListIndicesPaginateTypeDef definition

class ListIndicesRequestListIndicesPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessagesRequestListMessagesPaginateTypeDef

```python
# ListMessagesRequestListMessagesPaginateTypeDef definition

class ListMessagesRequestListMessagesPaginateTypeDef(TypedDict):
    conversationId: str,
    applicationId: str,
    userId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPluginsRequestListPluginsPaginateTypeDef

```python
# ListPluginsRequestListPluginsPaginateTypeDef definition

class ListPluginsRequestListPluginsPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRetrieversRequestListRetrieversPaginateTypeDef

```python
# ListRetrieversRequestListRetrieversPaginateTypeDef definition

class ListRetrieversRequestListRetrieversPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWebExperiencesRequestListWebExperiencesPaginateTypeDef

```python
# ListWebExperiencesRequestListWebExperiencesPaginateTypeDef definition

class ListWebExperiencesRequestListWebExperiencesPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GroupMembersTypeDef

```python
# GroupMembersTypeDef definition

class GroupMembersTypeDef(TypedDict):
    memberGroups: NotRequired[Sequence[MemberGroupTypeDef]],  # (1)
    memberUsers: NotRequired[Sequence[MemberUserTypeDef]],  # (2)
```

1. See [:material-code-braces: MemberGroupTypeDef](./type_defs.md#membergrouptypedef) 
2. See [:material-code-braces: MemberUserTypeDef](./type_defs.md#memberusertypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    items: List[GroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityProviderConfigurationTypeDef

```python
# IdentityProviderConfigurationTypeDef definition

class IdentityProviderConfigurationTypeDef(TypedDict):
    samlConfiguration: NotRequired[SamlProviderConfigurationTypeDef],  # (1)
    openIDConnectConfiguration: NotRequired[OpenIDConnectProviderConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SamlProviderConfigurationTypeDef](./type_defs.md#samlproviderconfigurationtypedef) 
2. See [:material-code-braces: OpenIDConnectProviderConfigurationTypeDef](./type_defs.md#openidconnectproviderconfigurationtypedef) 
## IndexStatisticsTypeDef

```python
# IndexStatisticsTypeDef definition

class IndexStatisticsTypeDef(TypedDict):
    textDocumentStatistics: NotRequired[TextDocumentStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef) 
## ListIndicesResponseTypeDef

```python
# ListIndicesResponseTypeDef definition

class ListIndicesResponseTypeDef(TypedDict):
    indices: List[IndexTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexTypeDef](./type_defs.md#indextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPluginsResponseTypeDef

```python
# ListPluginsResponseTypeDef definition

class ListPluginsResponseTypeDef(TypedDict):
    plugins: List[PluginTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PluginTypeDef](./type_defs.md#plugintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRetrieversResponseTypeDef

```python
# ListRetrieversResponseTypeDef definition

class ListRetrieversResponseTypeDef(TypedDict):
    retrievers: List[RetrieverTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RetrieverTypeDef](./type_defs.md#retrievertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebExperiencesResponseTypeDef

```python
# ListWebExperiencesResponseTypeDef definition

class ListWebExperiencesResponseTypeDef(TypedDict):
    webExperiences: List[WebExperienceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WebExperienceTypeDef](./type_defs.md#webexperiencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PluginAuthConfigurationOutputTypeDef

```python
# PluginAuthConfigurationOutputTypeDef definition

class PluginAuthConfigurationOutputTypeDef(TypedDict):
    basicAuthConfiguration: NotRequired[BasicAuthConfigurationTypeDef],  # (1)
    oAuth2ClientCredentialConfiguration: NotRequired[OAuth2ClientCredentialConfigurationTypeDef],  # (2)
    noAuthConfiguration: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef) 
2. See [:material-code-braces: OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef) 
## PluginAuthConfigurationTypeDef

```python
# PluginAuthConfigurationTypeDef definition

class PluginAuthConfigurationTypeDef(TypedDict):
    basicAuthConfiguration: NotRequired[BasicAuthConfigurationTypeDef],  # (1)
    oAuth2ClientCredentialConfiguration: NotRequired[OAuth2ClientCredentialConfigurationTypeDef],  # (2)
    noAuthConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef) 
2. See [:material-code-braces: OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef) 
## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    user: NotRequired[PrincipalUserTypeDef],  # (1)
    group: NotRequired[PrincipalGroupTypeDef],  # (2)
```

1. See [:material-code-braces: PrincipalUserTypeDef](./type_defs.md#principalusertypedef) 
2. See [:material-code-braces: PrincipalGroupTypeDef](./type_defs.md#principalgrouptypedef) 
## WebExperienceAuthConfigurationTypeDef

```python
# WebExperienceAuthConfigurationTypeDef definition

class WebExperienceAuthConfigurationTypeDef(TypedDict):
    samlConfiguration: NotRequired[SamlConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) 
## TextSegmentTypeDef

```python
# TextSegmentTypeDef definition

class TextSegmentTypeDef(TypedDict):
    beginOffset: NotRequired[int],
    endOffset: NotRequired[int],
    snippetExcerpt: NotRequired[SnippetExcerptTypeDef],  # (1)
```

1. See [:material-code-braces: SnippetExcerptTypeDef](./type_defs.md#snippetexcerpttypedef) 
## CustomPluginConfigurationTypeDef

```python
# CustomPluginConfigurationTypeDef definition

class CustomPluginConfigurationTypeDef(TypedDict):
    description: str,
    apiSchemaType: APISchemaTypeType,  # (1)
    apiSchema: APISchemaTypeDef,  # (2)
```

1. See [:material-code-brackets: APISchemaTypeType](./literals.md#apischematypetype) 
2. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
## ActionExecutionTypeDef

```python
# ActionExecutionTypeDef definition

class ActionExecutionTypeDef(TypedDict):
    pluginId: str,
    payload: Mapping[str, ActionExecutionPayloadFieldUnionTypeDef],  # (1)
    payloadFieldNameSeparator: str,
```

1. See [:material-code-braces: ActionExecutionPayloadFieldTypeDef](./type_defs.md#actionexecutionpayloadfieldtypedef) [:material-code-braces: ActionExecutionPayloadFieldOutputTypeDef](./type_defs.md#actionexecutionpayloadfieldoutputtypedef) 
## ActionReviewTypeDef

```python
# ActionReviewTypeDef definition

class ActionReviewTypeDef(TypedDict):
    pluginId: NotRequired[str],
    pluginType: NotRequired[PluginTypeType],  # (1)
    payload: NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],  # (2)
    payloadFieldNameSeparator: NotRequired[str],
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: ActionReviewPayloadFieldTypeDef](./type_defs.md#actionreviewpayloadfieldtypedef) 
## ListDocumentsResponseTypeDef

```python
# ListDocumentsResponseTypeDef definition

class ListDocumentsResponseTypeDef(TypedDict):
    documentDetailList: List[DocumentDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentDetailsTypeDef](./type_defs.md#documentdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDocumentResponseTypeDef

```python
# BatchDeleteDocumentResponseTypeDef definition

class BatchDeleteDocumentResponseTypeDef(TypedDict):
    failedDocuments: List[FailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutDocumentResponseTypeDef

```python
# BatchPutDocumentResponseTypeDef definition

class BatchPutDocumentResponseTypeDef(TypedDict):
    failedDocuments: List[FailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    status: GroupStatusDetailTypeDef,  # (1)
    statusHistory: List[GroupStatusDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef) 
2. See [:material-code-braces: GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleConfigurationOutputTypeDef

```python
# RuleConfigurationOutputTypeDef definition

class RuleConfigurationOutputTypeDef(TypedDict):
    contentBlockerRule: NotRequired[ContentBlockerRuleTypeDef],  # (1)
    contentRetrievalRule: NotRequired[ContentRetrievalRuleOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef) 
2. See [:material-code-braces: ContentRetrievalRuleOutputTypeDef](./type_defs.md#contentretrievalruleoutputtypedef) 
## ListDataSourceSyncJobsResponseTypeDef

```python
# ListDataSourceSyncJobsResponseTypeDef definition

class ListDataSourceSyncJobsResponseTypeDef(TypedDict):
    history: List[DataSourceSyncJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NativeIndexConfigurationOutputTypeDef

```python
# NativeIndexConfigurationOutputTypeDef definition

class NativeIndexConfigurationOutputTypeDef(TypedDict):
    indexId: str,
    boostingOverride: NotRequired[Dict[str, DocumentAttributeBoostingConfigurationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#documentattributeboostingconfigurationoutputtypedef) 
## HookConfigurationOutputTypeDef

```python
# HookConfigurationOutputTypeDef definition

class HookConfigurationOutputTypeDef(TypedDict):
    invocationCondition: NotRequired[DocumentAttributeConditionOutputTypeDef],  # (1)
    lambdaArn: NotRequired[str],
    s3BucketName: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
## InlineDocumentEnrichmentConfigurationOutputTypeDef

```python
# InlineDocumentEnrichmentConfigurationOutputTypeDef definition

class InlineDocumentEnrichmentConfigurationOutputTypeDef(TypedDict):
    condition: NotRequired[DocumentAttributeConditionOutputTypeDef],  # (1)
    target: NotRequired[DocumentAttributeTargetOutputTypeDef],  # (2)
    documentContentOperator: NotRequired[DocumentContentOperatorType],  # (3)
```

1. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 
3. See [:material-code-brackets: DocumentContentOperatorType](./literals.md#documentcontentoperatortype) 
## PutFeedbackRequestRequestTypeDef

```python
# PutFeedbackRequestRequestTypeDef definition

class PutFeedbackRequestRequestTypeDef(TypedDict):
    applicationId: str,
    conversationId: str,
    messageId: str,
    userId: NotRequired[str],
    messageCopiedAt: NotRequired[TimestampTypeDef],
    messageUsefulness: NotRequired[MessageUsefulnessFeedbackTypeDef],  # (1)
```

1. See [:material-code-braces: MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef) 
## PutGroupRequestRequestTypeDef

```python
# PutGroupRequestRequestTypeDef definition

class PutGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    groupName: str,
    type: MembershipTypeType,  # (1)
    groupMembers: GroupMembersTypeDef,  # (2)
    dataSourceId: NotRequired[str],
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
2. See [:material-code-braces: GroupMembersTypeDef](./type_defs.md#groupmemberstypedef) 
## CreateWebExperienceRequestRequestTypeDef

```python
# CreateWebExperienceRequestRequestTypeDef definition

class CreateWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    title: NotRequired[str],
    subtitle: NotRequired[str],
    welcomeMessage: NotRequired[str],
    samplePromptsControlMode: NotRequired[WebExperienceSamplePromptsControlModeType],  # (1)
    origins: NotRequired[Sequence[str]],
    roleArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    clientToken: NotRequired[str],
    identityProviderConfiguration: NotRequired[IdentityProviderConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef) 
## GetIndexResponseTypeDef

```python
# GetIndexResponseTypeDef definition

class GetIndexResponseTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    displayName: str,
    type: IndexTypeType,  # (1)
    indexArn: str,
    status: IndexStatusType,  # (2)
    description: str,
    createdAt: datetime,
    updatedAt: datetime,
    capacityConfiguration: IndexCapacityConfigurationTypeDef,  # (3)
    documentAttributeConfigurations: List[DocumentAttributeConfigurationTypeDef],  # (4)
    error: ErrorDetailTypeDef,  # (5)
    indexStatistics: IndexStatisticsTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
3. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
4. See [:material-code-braces: DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef) 
5. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
6. See [:material-code-braces: IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccessControlTypeDef

```python
# AccessControlTypeDef definition

class AccessControlTypeDef(TypedDict):
    principals: Sequence[PrincipalTypeDef],  # (1)
    memberRelation: NotRequired[MemberRelationType],  # (2)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-brackets: MemberRelationType](./literals.md#memberrelationtype) 
## GetWebExperienceResponseTypeDef

```python
# GetWebExperienceResponseTypeDef definition

class GetWebExperienceResponseTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
    webExperienceArn: str,
    defaultEndpoint: str,
    status: WebExperienceStatusType,  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    title: str,
    subtitle: str,
    welcomeMessage: str,
    samplePromptsControlMode: WebExperienceSamplePromptsControlModeType,  # (2)
    origins: List[str],
    roleArn: str,
    identityProviderConfiguration: IdentityProviderConfigurationTypeDef,  # (3)
    authenticationConfiguration: WebExperienceAuthConfigurationTypeDef,  # (4)
    error: ErrorDetailTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: WebExperienceStatusType](./literals.md#webexperiencestatustype) 
2. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
3. See [:material-code-braces: IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef) 
4. See [:material-code-braces: WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef) 
5. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebExperienceRequestRequestTypeDef

```python
# UpdateWebExperienceRequestRequestTypeDef definition

class UpdateWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
    roleArn: NotRequired[str],
    authenticationConfiguration: NotRequired[WebExperienceAuthConfigurationTypeDef],  # (1)
    title: NotRequired[str],
    subtitle: NotRequired[str],
    welcomeMessage: NotRequired[str],
    samplePromptsControlMode: NotRequired[WebExperienceSamplePromptsControlModeType],  # (2)
    identityProviderConfiguration: NotRequired[IdentityProviderConfigurationTypeDef],  # (3)
    origins: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef) 
2. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
3. See [:material-code-braces: IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef) 
## SourceAttributionTypeDef

```python
# SourceAttributionTypeDef definition

class SourceAttributionTypeDef(TypedDict):
    title: NotRequired[str],
    snippet: NotRequired[str],
    url: NotRequired[str],
    citationNumber: NotRequired[int],
    updatedAt: NotRequired[datetime],
    textMessageSegments: NotRequired[List[TextSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: TextSegmentTypeDef](./type_defs.md#textsegmenttypedef) 
## DocumentAttributeBoostingConfigurationTypeDef

```python
# DocumentAttributeBoostingConfigurationTypeDef definition

class DocumentAttributeBoostingConfigurationTypeDef(TypedDict):
    numberConfiguration: NotRequired[NumberAttributeBoostingConfigurationTypeDef],  # (1)
    stringConfiguration: NotRequired[StringAttributeBoostingConfigurationUnionTypeDef],  # (2)
    dateConfiguration: NotRequired[DateAttributeBoostingConfigurationTypeDef],  # (3)
    stringListConfiguration: NotRequired[StringListAttributeBoostingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: NumberAttributeBoostingConfigurationTypeDef](./type_defs.md#numberattributeboostingconfigurationtypedef) 
2. See [:material-code-braces: StringAttributeBoostingConfigurationTypeDef](./type_defs.md#stringattributeboostingconfigurationtypedef) [:material-code-braces: StringAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#stringattributeboostingconfigurationoutputtypedef) 
3. See [:material-code-braces: DateAttributeBoostingConfigurationTypeDef](./type_defs.md#dateattributeboostingconfigurationtypedef) 
4. See [:material-code-braces: StringListAttributeBoostingConfigurationTypeDef](./type_defs.md#stringlistattributeboostingconfigurationtypedef) 
## CreatePluginRequestRequestTypeDef

```python
# CreatePluginRequestRequestTypeDef definition

class CreatePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    displayName: str,
    type: PluginTypeType,  # (1)
    authConfiguration: PluginAuthConfigurationTypeDef,  # (2)
    serverUrl: NotRequired[str],
    customPluginConfiguration: NotRequired[CustomPluginConfigurationTypeDef],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
3. See [:material-code-braces: CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetPluginResponseTypeDef

```python
# GetPluginResponseTypeDef definition

class GetPluginResponseTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
    displayName: str,
    type: PluginTypeType,  # (1)
    serverUrl: str,
    authConfiguration: PluginAuthConfigurationOutputTypeDef,  # (2)
    customPluginConfiguration: CustomPluginConfigurationTypeDef,  # (3)
    buildStatus: PluginBuildStatusType,  # (4)
    pluginArn: str,
    state: PluginStateType,  # (5)
    createdAt: datetime,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: PluginAuthConfigurationOutputTypeDef](./type_defs.md#pluginauthconfigurationoutputtypedef) 
3. See [:material-code-braces: CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef) 
4. See [:material-code-brackets: PluginBuildStatusType](./literals.md#pluginbuildstatustype) 
5. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePluginRequestRequestTypeDef

```python
# UpdatePluginRequestRequestTypeDef definition

class UpdatePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
    displayName: NotRequired[str],
    state: NotRequired[PluginStateType],  # (1)
    serverUrl: NotRequired[str],
    customPluginConfiguration: NotRequired[CustomPluginConfigurationTypeDef],  # (2)
    authConfiguration: NotRequired[PluginAuthConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
2. See [:material-code-braces: CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef) 
3. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
## RuleOutputTypeDef

```python
# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    ruleType: RuleTypeType,  # (3)
    includedUsersAndGroups: NotRequired[UsersAndGroupsOutputTypeDef],  # (1)
    excludedUsersAndGroups: NotRequired[UsersAndGroupsOutputTypeDef],  # (1)
    ruleConfiguration: NotRequired[RuleConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef) 
2. See [:material-code-braces: UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: RuleConfigurationOutputTypeDef](./type_defs.md#ruleconfigurationoutputtypedef) 
## RuleConfigurationTypeDef

```python
# RuleConfigurationTypeDef definition

class RuleConfigurationTypeDef(TypedDict):
    contentBlockerRule: NotRequired[ContentBlockerRuleTypeDef],  # (1)
    contentRetrievalRule: NotRequired[ContentRetrievalRuleUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef) 
2. See [:material-code-braces: ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef) [:material-code-braces: ContentRetrievalRuleOutputTypeDef](./type_defs.md#contentretrievalruleoutputtypedef) 
## RetrieverConfigurationOutputTypeDef

```python
# RetrieverConfigurationOutputTypeDef definition

class RetrieverConfigurationOutputTypeDef(TypedDict):
    nativeIndexConfiguration: NotRequired[NativeIndexConfigurationOutputTypeDef],  # (1)
    kendraIndexConfiguration: NotRequired[KendraIndexConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: NativeIndexConfigurationOutputTypeDef](./type_defs.md#nativeindexconfigurationoutputtypedef) 
2. See [:material-code-braces: KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef) 
## DocumentEnrichmentConfigurationOutputTypeDef

```python
# DocumentEnrichmentConfigurationOutputTypeDef definition

class DocumentEnrichmentConfigurationOutputTypeDef(TypedDict):
    inlineConfigurations: NotRequired[List[InlineDocumentEnrichmentConfigurationOutputTypeDef]],  # (1)
    preExtractionHookConfiguration: NotRequired[HookConfigurationOutputTypeDef],  # (2)
    postExtractionHookConfiguration: NotRequired[HookConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: InlineDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationoutputtypedef) 
2. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
3. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
## DocumentAttributeConditionTypeDef

```python
# DocumentAttributeConditionTypeDef definition

class DocumentAttributeConditionTypeDef(TypedDict):
    key: str,
    operator: DocumentEnrichmentConditionOperatorType,  # (1)
    value: NotRequired[DocumentAttributeValueUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: DocumentEnrichmentConditionOperatorType](./literals.md#documentenrichmentconditionoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeTargetTypeDef

```python
# DocumentAttributeTargetTypeDef definition

class DocumentAttributeTargetTypeDef(TypedDict):
    key: str,
    value: NotRequired[DocumentAttributeValueUnionTypeDef],  # (1)
    attributeValueOperator: NotRequired[AttributeValueOperatorType],  # (2)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
2. See [:material-code-brackets: AttributeValueOperatorType](./literals.md#attributevalueoperatortype) 
## DocumentAttributeTypeDef

```python
# DocumentAttributeTypeDef definition

class DocumentAttributeTypeDef(TypedDict):
    name: str,
    value: DocumentAttributeValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## AccessConfigurationTypeDef

```python
# AccessConfigurationTypeDef definition

class AccessConfigurationTypeDef(TypedDict):
    accessControls: Sequence[AccessControlTypeDef],  # (1)
    memberRelation: NotRequired[MemberRelationType],  # (2)
```

1. See [:material-code-braces: AccessControlTypeDef](./type_defs.md#accesscontroltypedef) 
2. See [:material-code-brackets: MemberRelationType](./literals.md#memberrelationtype) 
## ChatSyncOutputTypeDef

```python
# ChatSyncOutputTypeDef definition

class ChatSyncOutputTypeDef(TypedDict):
    conversationId: str,
    systemMessage: str,
    systemMessageId: str,
    userMessageId: str,
    actionReview: ActionReviewTypeDef,  # (1)
    authChallengeRequest: AuthChallengeRequestTypeDef,  # (2)
    sourceAttributions: List[SourceAttributionTypeDef],  # (3)
    failedAttachments: List[AttachmentOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ActionReviewTypeDef](./type_defs.md#actionreviewtypedef) 
2. See [:material-code-braces: AuthChallengeRequestTypeDef](./type_defs.md#authchallengerequesttypedef) 
3. See [:material-code-braces: SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef) 
4. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    messageId: NotRequired[str],
    body: NotRequired[str],
    time: NotRequired[datetime],
    type: NotRequired[MessageTypeType],  # (1)
    attachments: NotRequired[List[AttachmentOutputTypeDef]],  # (2)
    sourceAttribution: NotRequired[List[SourceAttributionTypeDef]],  # (3)
    actionReview: NotRequired[ActionReviewTypeDef],  # (4)
    actionExecution: NotRequired[ActionExecutionOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
3. See [:material-code-braces: SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef) 
4. See [:material-code-braces: ActionReviewTypeDef](./type_defs.md#actionreviewtypedef) 
5. See [:material-code-braces: ActionExecutionOutputTypeDef](./type_defs.md#actionexecutionoutputtypedef) 
## TopicConfigurationOutputTypeDef

```python
# TopicConfigurationOutputTypeDef definition

class TopicConfigurationOutputTypeDef(TypedDict):
    name: str,
    rules: List[RuleOutputTypeDef],  # (1)
    description: NotRequired[str],
    exampleChatMessages: NotRequired[List[str]],
```

1. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## GetRetrieverResponseTypeDef

```python
# GetRetrieverResponseTypeDef definition

class GetRetrieverResponseTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
    retrieverArn: str,
    type: RetrieverTypeType,  # (1)
    status: RetrieverStatusType,  # (2)
    displayName: str,
    configuration: RetrieverConfigurationOutputTypeDef,  # (3)
    roleArn: str,
    createdAt: datetime,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
2. See [:material-code-brackets: RetrieverStatusType](./literals.md#retrieverstatustype) 
3. See [:material-code-braces: RetrieverConfigurationOutputTypeDef](./type_defs.md#retrieverconfigurationoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataSourceResponseTypeDef

```python
# GetDataSourceResponseTypeDef definition

class GetDataSourceResponseTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceId: str,
    dataSourceArn: str,
    displayName: str,
    type: str,
    configuration: Dict[str, Any],
    vpcConfiguration: DataSourceVpcConfigurationOutputTypeDef,  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    description: str,
    status: DataSourceStatusType,  # (2)
    syncSchedule: str,
    roleArn: str,
    error: ErrorDetailTypeDef,  # (3)
    documentEnrichmentConfiguration: DocumentEnrichmentConfigurationOutputTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
2. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-braces: DocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#documentenrichmentconfigurationoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttributeFilterTypeDef

```python
# AttributeFilterTypeDef definition

class AttributeFilterTypeDef(TypedDict):
    andAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    orAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    notFilter: NotRequired[Mapping[str, Any]],
    equalsTo: NotRequired[DocumentAttributeTypeDef],  # (1)
    containsAll: NotRequired[DocumentAttributeTypeDef],  # (1)
    containsAny: NotRequired[DocumentAttributeTypeDef],  # (1)
    greaterThan: NotRequired[DocumentAttributeTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[DocumentAttributeTypeDef],  # (1)
    lessThan: NotRequired[DocumentAttributeTypeDef],  # (1)
    lessThanOrEquals: NotRequired[DocumentAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
3. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
4. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
5. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
6. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
7. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
## ListMessagesResponseTypeDef

```python
# ListMessagesResponseTypeDef definition

class ListMessagesResponseTypeDef(TypedDict):
    messages: List[MessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NativeIndexConfigurationTypeDef

```python
# NativeIndexConfigurationTypeDef definition

class NativeIndexConfigurationTypeDef(TypedDict):
    indexId: str,
    boostingOverride: NotRequired[Mapping[str, DocumentAttributeBoostingConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentAttributeBoostingConfigurationTypeDef](./type_defs.md#documentattributeboostingconfigurationtypedef) [:material-code-braces: DocumentAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#documentattributeboostingconfigurationoutputtypedef) 
## GetChatControlsConfigurationResponseTypeDef

```python
# GetChatControlsConfigurationResponseTypeDef definition

class GetChatControlsConfigurationResponseTypeDef(TypedDict):
    responseScope: ResponseScopeType,  # (1)
    blockedPhrases: BlockedPhrasesConfigurationTypeDef,  # (2)
    topicConfigurations: List[TopicConfigurationOutputTypeDef],  # (3)
    creatorModeConfiguration: AppliedCreatorModeConfigurationTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResponseScopeType](./literals.md#responsescopetype) 
2. See [:material-code-braces: BlockedPhrasesConfigurationTypeDef](./type_defs.md#blockedphrasesconfigurationtypedef) 
3. See [:material-code-braces: TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef) 
4. See [:material-code-braces: AppliedCreatorModeConfigurationTypeDef](./type_defs.md#appliedcreatormodeconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    ruleType: RuleTypeType,  # (3)
    includedUsersAndGroups: NotRequired[UsersAndGroupsUnionTypeDef],  # (1)
    excludedUsersAndGroups: NotRequired[UsersAndGroupsUnionTypeDef],  # (1)
    ruleConfiguration: NotRequired[RuleConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef) [:material-code-braces: UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef) 
2. See [:material-code-braces: UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef) [:material-code-braces: UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef) [:material-code-braces: RuleConfigurationOutputTypeDef](./type_defs.md#ruleconfigurationoutputtypedef) 
## HookConfigurationTypeDef

```python
# HookConfigurationTypeDef definition

class HookConfigurationTypeDef(TypedDict):
    invocationCondition: NotRequired[DocumentAttributeConditionUnionTypeDef],  # (1)
    lambdaArn: NotRequired[str],
    s3BucketName: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
## InlineDocumentEnrichmentConfigurationTypeDef

```python
# InlineDocumentEnrichmentConfigurationTypeDef definition

class InlineDocumentEnrichmentConfigurationTypeDef(TypedDict):
    condition: NotRequired[DocumentAttributeConditionUnionTypeDef],  # (1)
    target: NotRequired[DocumentAttributeTargetUnionTypeDef],  # (2)
    documentContentOperator: NotRequired[DocumentContentOperatorType],  # (3)
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef) [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 
3. See [:material-code-brackets: DocumentContentOperatorType](./literals.md#documentcontentoperatortype) 
## ChatSyncInputRequestTypeDef

```python
# ChatSyncInputRequestTypeDef definition

class ChatSyncInputRequestTypeDef(TypedDict):
    applicationId: str,
    userId: NotRequired[str],
    userGroups: NotRequired[Sequence[str]],
    userMessage: NotRequired[str],
    attachments: NotRequired[Sequence[AttachmentInputTypeDef]],  # (1)
    actionExecution: NotRequired[ActionExecutionTypeDef],  # (2)
    authChallengeResponse: NotRequired[AuthChallengeResponseTypeDef],  # (3)
    conversationId: NotRequired[str],
    parentMessageId: NotRequired[str],
    attributeFilter: NotRequired[AttributeFilterTypeDef],  # (4)
    chatMode: NotRequired[ChatModeType],  # (5)
    chatModeConfiguration: NotRequired[ChatModeConfigurationTypeDef],  # (6)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef) 
2. See [:material-code-braces: ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef) 
3. See [:material-code-braces: AuthChallengeResponseTypeDef](./type_defs.md#authchallengeresponsetypedef) 
4. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
5. See [:material-code-brackets: ChatModeType](./literals.md#chatmodetype) 
6. See [:material-code-braces: ChatModeConfigurationTypeDef](./type_defs.md#chatmodeconfigurationtypedef) 
## RetrieverConfigurationTypeDef

```python
# RetrieverConfigurationTypeDef definition

class RetrieverConfigurationTypeDef(TypedDict):
    nativeIndexConfiguration: NotRequired[NativeIndexConfigurationUnionTypeDef],  # (1)
    kendraIndexConfiguration: NotRequired[KendraIndexConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef) [:material-code-braces: NativeIndexConfigurationOutputTypeDef](./type_defs.md#nativeindexconfigurationoutputtypedef) 
2. See [:material-code-braces: KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef) 
## TopicConfigurationTypeDef

```python
# TopicConfigurationTypeDef definition

class TopicConfigurationTypeDef(TypedDict):
    name: str,
    rules: Sequence[RuleUnionTypeDef],  # (1)
    description: NotRequired[str],
    exampleChatMessages: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## DocumentEnrichmentConfigurationTypeDef

```python
# DocumentEnrichmentConfigurationTypeDef definition

class DocumentEnrichmentConfigurationTypeDef(TypedDict):
    inlineConfigurations: NotRequired[Sequence[InlineDocumentEnrichmentConfigurationUnionTypeDef]],  # (1)
    preExtractionHookConfiguration: NotRequired[HookConfigurationUnionTypeDef],  # (2)
    postExtractionHookConfiguration: NotRequired[HookConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef) [:material-code-braces: InlineDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationoutputtypedef) 
2. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
3. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
## CreateRetrieverRequestRequestTypeDef

```python
# CreateRetrieverRequestRequestTypeDef definition

class CreateRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    type: RetrieverTypeType,  # (1)
    displayName: str,
    configuration: RetrieverConfigurationTypeDef,  # (2)
    roleArn: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
2. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRetrieverRequestRequestTypeDef

```python
# UpdateRetrieverRequestRequestTypeDef definition

class UpdateRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
    configuration: NotRequired[RetrieverConfigurationTypeDef],  # (1)
    displayName: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    displayName: str,
    configuration: Mapping[str, Any],
    vpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    syncSchedule: NotRequired[str],
    roleArn: NotRequired[str],
    clientToken: NotRequired[str],
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceId: str,
    displayName: NotRequired[str],
    configuration: NotRequired[Mapping[str, Any]],
    vpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    syncSchedule: NotRequired[str],
    roleArn: NotRequired[str],
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
2. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
## UpdateChatControlsConfigurationRequestRequestTypeDef

```python
# UpdateChatControlsConfigurationRequestRequestTypeDef definition

class UpdateChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    clientToken: NotRequired[str],
    responseScope: NotRequired[ResponseScopeType],  # (1)
    blockedPhrasesConfigurationUpdate: NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],  # (2)
    topicConfigurationsToCreateOrUpdate: NotRequired[Sequence[TopicConfigurationUnionTypeDef]],  # (3)
    topicConfigurationsToDelete: NotRequired[Sequence[TopicConfigurationTypeDef]],  # (4)
    creatorModeConfiguration: NotRequired[CreatorModeConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: ResponseScopeType](./literals.md#responsescopetype) 
2. See [:material-code-braces: BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef) 
3. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) [:material-code-braces: TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef) 
4. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
5. See [:material-code-braces: CreatorModeConfigurationTypeDef](./type_defs.md#creatormodeconfigurationtypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    id: str,
    attributes: NotRequired[Sequence[DocumentAttributeTypeDef]],  # (1)
    content: NotRequired[DocumentContentTypeDef],  # (2)
    contentType: NotRequired[ContentTypeType],  # (3)
    title: NotRequired[str],
    accessConfiguration: NotRequired[AccessConfigurationTypeDef],  # (4)
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationUnionTypeDef],  # (5)
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
2. See [:material-code-braces: DocumentContentTypeDef](./type_defs.md#documentcontenttypedef) 
3. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
4. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
5. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) [:material-code-braces: DocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#documentenrichmentconfigurationoutputtypedef) 
## BatchPutDocumentRequestRequestTypeDef

```python
# BatchPutDocumentRequestRequestTypeDef definition

class BatchPutDocumentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    documents: Sequence[DocumentTypeDef],  # (1)
    roleArn: NotRequired[str],
    dataSourceSyncId: NotRequired[str],
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
