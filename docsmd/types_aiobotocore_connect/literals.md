# Literals

> [Index](../README.md) > [Connect](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## AccessTypeType

```python
# AccessTypeType usage example
from types_aiobotocore_connect.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "ALLOW"
```

```python
# AccessTypeType definition
AccessTypeType = Literal[
    "ALLOW",
]
```
## ActionTypeType

```python
# ActionTypeType usage example
from types_aiobotocore_connect.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "ASSIGN_CONTACT_CATEGORY"
```

```python
# ActionTypeType definition
ActionTypeType = Literal[
    "ASSIGN_CONTACT_CATEGORY",
    "ASSIGN_SLA",
    "CREATE_CASE",
    "CREATE_TASK",
    "END_ASSOCIATED_TASKS",
    "GENERATE_EVENTBRIDGE_EVENT",
    "SEND_NOTIFICATION",
    "SUBMIT_AUTO_EVALUATION",
    "UPDATE_CASE",
]
```
## AgentAvailabilityTimerType

```python
# AgentAvailabilityTimerType usage example
from types_aiobotocore_connect.literals import AgentAvailabilityTimerType

def get_value() -> AgentAvailabilityTimerType:
    return "TIME_SINCE_LAST_ACTIVITY"
```

```python
# AgentAvailabilityTimerType definition
AgentAvailabilityTimerType = Literal[
    "TIME_SINCE_LAST_ACTIVITY",
    "TIME_SINCE_LAST_INBOUND",
]
```
## AgentStatusStateType

```python
# AgentStatusStateType usage example
from types_aiobotocore_connect.literals import AgentStatusStateType

def get_value() -> AgentStatusStateType:
    return "DISABLED"
```

```python
# AgentStatusStateType definition
AgentStatusStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AgentStatusTypeType

```python
# AgentStatusTypeType usage example
from types_aiobotocore_connect.literals import AgentStatusTypeType

def get_value() -> AgentStatusTypeType:
    return "CUSTOM"
```

```python
# AgentStatusTypeType definition
AgentStatusTypeType = Literal[
    "CUSTOM",
    "OFFLINE",
    "ROUTABLE",
]
```
## AiUseCaseType

```python
# AiUseCaseType usage example
from types_aiobotocore_connect.literals import AiUseCaseType

def get_value() -> AiUseCaseType:
    return "AgentAssistance"
```

```python
# AiUseCaseType definition
AiUseCaseType = Literal[
    "AgentAssistance",
    "SelfService",
]
```
## AllowedUserActionType

```python
# AllowedUserActionType usage example
from types_aiobotocore_connect.literals import AllowedUserActionType

def get_value() -> AllowedUserActionType:
    return "CALL"
```

```python
# AllowedUserActionType definition
AllowedUserActionType = Literal[
    "CALL",
    "DISCARD",
]
```
## AnsweringMachineDetectionStatusType

```python
# AnsweringMachineDetectionStatusType usage example
from types_aiobotocore_connect.literals import AnsweringMachineDetectionStatusType

def get_value() -> AnsweringMachineDetectionStatusType:
    return "AMD_ERROR"
```

```python
# AnsweringMachineDetectionStatusType definition
AnsweringMachineDetectionStatusType = Literal[
    "AMD_ERROR",
    "AMD_NOT_APPLICABLE",
    "AMD_UNANSWERED",
    "AMD_UNRESOLVED",
    "ANSWERED",
    "ERROR",
    "FAX_MACHINE_DETECTED",
    "HUMAN_ANSWERED",
    "SIT_TONE_BUSY",
    "SIT_TONE_DETECTED",
    "SIT_TONE_INVALID_NUMBER",
    "UNDETECTED",
    "VOICEMAIL_BEEP",
    "VOICEMAIL_NO_BEEP",
]
```
## ApplicationTypeType

```python
# ApplicationTypeType usage example
from types_aiobotocore_connect.literals import ApplicationTypeType

def get_value() -> ApplicationTypeType:
    return "MCP"
```

```python
# ApplicationTypeType definition
ApplicationTypeType = Literal[
    "MCP",
    "THIRD_PARTY_APPLICATION",
]
```
## ArtifactStatusType

```python
# ArtifactStatusType usage example
from types_aiobotocore_connect.literals import ArtifactStatusType

def get_value() -> ArtifactStatusType:
    return "APPROVED"
```

```python
# ArtifactStatusType definition
ArtifactStatusType = Literal[
    "APPROVED",
    "IN_PROGRESS",
    "REJECTED",
]
```
## AutoEvaluationStatusType

```python
# AutoEvaluationStatusType usage example
from types_aiobotocore_connect.literals import AutoEvaluationStatusType

def get_value() -> AutoEvaluationStatusType:
    return "FAILED"
```

```python
# AutoEvaluationStatusType definition
AutoEvaluationStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCEEDED",
]
```
## BehaviorTypeType

```python
# BehaviorTypeType usage example
from types_aiobotocore_connect.literals import BehaviorTypeType

def get_value() -> BehaviorTypeType:
    return "ROUTE_ANY_CHANNEL"
```

```python
# BehaviorTypeType definition
BehaviorTypeType = Literal[
    "ROUTE_ANY_CHANNEL",
    "ROUTE_CURRENT_CHANNEL_ONLY",
]
```
## BooleanComparisonTypeType

```python
# BooleanComparisonTypeType usage example
from types_aiobotocore_connect.literals import BooleanComparisonTypeType

def get_value() -> BooleanComparisonTypeType:
    return "IS_FALSE"
```

```python
# BooleanComparisonTypeType definition
BooleanComparisonTypeType = Literal[
    "IS_FALSE",
    "IS_TRUE",
]
```
## ChannelType

```python
# ChannelType usage example
from types_aiobotocore_connect.literals import ChannelType

def get_value() -> ChannelType:
    return "CHAT"
```

```python
# ChannelType definition
ChannelType = Literal[
    "CHAT",
    "EMAIL",
    "TASK",
    "VOICE",
]
```
## ChatEventTypeType

```python
# ChatEventTypeType usage example
from types_aiobotocore_connect.literals import ChatEventTypeType

def get_value() -> ChatEventTypeType:
    return "DISCONNECT"
```

```python
# ChatEventTypeType definition
ChatEventTypeType = Literal[
    "DISCONNECT",
    "EVENT",
    "MESSAGE",
]
```
## ComparisonType

```python
# ComparisonType usage example
from types_aiobotocore_connect.literals import ComparisonType

def get_value() -> ComparisonType:
    return "LT"
```

```python
# ComparisonType definition
ComparisonType = Literal[
    "LT",
]
```
## ContactFlowModuleStateType

```python
# ContactFlowModuleStateType usage example
from types_aiobotocore_connect.literals import ContactFlowModuleStateType

def get_value() -> ContactFlowModuleStateType:
    return "ACTIVE"
```

```python
# ContactFlowModuleStateType definition
ContactFlowModuleStateType = Literal[
    "ACTIVE",
    "ARCHIVED",
]
```
## ContactFlowModuleStatusType

```python
# ContactFlowModuleStatusType usage example
from types_aiobotocore_connect.literals import ContactFlowModuleStatusType

def get_value() -> ContactFlowModuleStatusType:
    return "PUBLISHED"
```

```python
# ContactFlowModuleStatusType definition
ContactFlowModuleStatusType = Literal[
    "PUBLISHED",
    "SAVED",
]
```
## ContactFlowStateType

```python
# ContactFlowStateType usage example
from types_aiobotocore_connect.literals import ContactFlowStateType

def get_value() -> ContactFlowStateType:
    return "ACTIVE"
```

```python
# ContactFlowStateType definition
ContactFlowStateType = Literal[
    "ACTIVE",
    "ARCHIVED",
]
```
## ContactFlowStatusType

```python
# ContactFlowStatusType usage example
from types_aiobotocore_connect.literals import ContactFlowStatusType

def get_value() -> ContactFlowStatusType:
    return "PUBLISHED"
```

```python
# ContactFlowStatusType definition
ContactFlowStatusType = Literal[
    "PUBLISHED",
    "SAVED",
]
```
## ContactFlowTypeType

```python
# ContactFlowTypeType usage example
from types_aiobotocore_connect.literals import ContactFlowTypeType

def get_value() -> ContactFlowTypeType:
    return "AGENT_HOLD"
```

```python
# ContactFlowTypeType definition
ContactFlowTypeType = Literal[
    "AGENT_HOLD",
    "AGENT_TRANSFER",
    "AGENT_WHISPER",
    "CAMPAIGN",
    "CONTACT_FLOW",
    "CUSTOMER_HOLD",
    "CUSTOMER_QUEUE",
    "CUSTOMER_WHISPER",
    "OUTBOUND_WHISPER",
    "QUEUE_TRANSFER",
]
```
## ContactInitiationMethodType

```python
# ContactInitiationMethodType usage example
from types_aiobotocore_connect.literals import ContactInitiationMethodType

def get_value() -> ContactInitiationMethodType:
    return "AGENT_REPLY"
```

```python
# ContactInitiationMethodType definition
ContactInitiationMethodType = Literal[
    "AGENT_REPLY",
    "API",
    "CALLBACK",
    "DISCONNECT",
    "EXTERNAL_OUTBOUND",
    "FLOW",
    "INBOUND",
    "MONITOR",
    "OUTBOUND",
    "QUEUE_TRANSFER",
    "TRANSFER",
    "WEBRTC_API",
]
```
## ContactInteractionTypeType

```python
# ContactInteractionTypeType usage example
from types_aiobotocore_connect.literals import ContactInteractionTypeType

def get_value() -> ContactInteractionTypeType:
    return "AGENT"
```

```python
# ContactInteractionTypeType definition
ContactInteractionTypeType = Literal[
    "AGENT",
    "AUTOMATED",
]
```
## ContactMediaProcessingFailureModeType

```python
# ContactMediaProcessingFailureModeType usage example
from types_aiobotocore_connect.literals import ContactMediaProcessingFailureModeType

def get_value() -> ContactMediaProcessingFailureModeType:
    return "DELIVER_UNPROCESSED_MESSAGE"
```

```python
# ContactMediaProcessingFailureModeType definition
ContactMediaProcessingFailureModeType = Literal[
    "DELIVER_UNPROCESSED_MESSAGE",
    "DO_NOT_DELIVER_UNPROCESSED_MESSAGE",
]
```
## ContactMetricNameType

```python
# ContactMetricNameType usage example
from types_aiobotocore_connect.literals import ContactMetricNameType

def get_value() -> ContactMetricNameType:
    return "POSITION_IN_QUEUE"
```

```python
# ContactMetricNameType definition
ContactMetricNameType = Literal[
    "POSITION_IN_QUEUE",
]
```
## ContactParticipantRoleType

```python
# ContactParticipantRoleType usage example
from types_aiobotocore_connect.literals import ContactParticipantRoleType

def get_value() -> ContactParticipantRoleType:
    return "AGENT"
```

```python
# ContactParticipantRoleType definition
ContactParticipantRoleType = Literal[
    "AGENT",
    "CUSTOM_BOT",
    "SYSTEM",
]
```
## ContactRecordingTypeType

```python
# ContactRecordingTypeType usage example
from types_aiobotocore_connect.literals import ContactRecordingTypeType

def get_value() -> ContactRecordingTypeType:
    return "AGENT"
```

```python
# ContactRecordingTypeType definition
ContactRecordingTypeType = Literal[
    "AGENT",
    "IVR",
    "SCREEN",
]
```
## ContactStateType

```python
# ContactStateType usage example
from types_aiobotocore_connect.literals import ContactStateType

def get_value() -> ContactStateType:
    return "CONNECTED"
```

```python
# ContactStateType definition
ContactStateType = Literal[
    "CONNECTED",
    "CONNECTED_ONHOLD",
    "CONNECTING",
    "ENDED",
    "ERROR",
    "INCOMING",
    "MISSED",
    "PENDING",
    "REJECTED",
]
```
## CurrentMetricNameType

```python
# CurrentMetricNameType usage example
from types_aiobotocore_connect.literals import CurrentMetricNameType

def get_value() -> CurrentMetricNameType:
    return "AGENTS_AFTER_CONTACT_WORK"
```

```python
# CurrentMetricNameType definition
CurrentMetricNameType = Literal[
    "AGENTS_AFTER_CONTACT_WORK",
    "AGENTS_AVAILABLE",
    "AGENTS_ERROR",
    "AGENTS_NON_PRODUCTIVE",
    "AGENTS_ON_CALL",
    "AGENTS_ON_CONTACT",
    "AGENTS_ONLINE",
    "AGENTS_STAFFED",
    "CONTACTS_IN_QUEUE",
    "CONTACTS_SCHEDULED",
    "OLDEST_CONTACT_AGE",
    "SLOTS_ACTIVE",
    "SLOTS_AVAILABLE",
]
```
## DataTableAttributeValueTypeType

```python
# DataTableAttributeValueTypeType usage example
from types_aiobotocore_connect.literals import DataTableAttributeValueTypeType

def get_value() -> DataTableAttributeValueTypeType:
    return "BOOLEAN"
```

```python
# DataTableAttributeValueTypeType definition
DataTableAttributeValueTypeType = Literal[
    "BOOLEAN",
    "NUMBER",
    "NUMBER_LIST",
    "TEXT",
    "TEXT_LIST",
]
```
## DataTableLockLevelType

```python
# DataTableLockLevelType usage example
from types_aiobotocore_connect.literals import DataTableLockLevelType

def get_value() -> DataTableLockLevelType:
    return "ATTRIBUTE"
```

```python
# DataTableLockLevelType definition
DataTableLockLevelType = Literal[
    "ATTRIBUTE",
    "DATA_TABLE",
    "NONE",
    "PRIMARY_VALUE",
    "VALUE",
]
```
## DataTableStatusType

```python
# DataTableStatusType usage example
from types_aiobotocore_connect.literals import DataTableStatusType

def get_value() -> DataTableStatusType:
    return "PUBLISHED"
```

```python
# DataTableStatusType definition
DataTableStatusType = Literal[
    "PUBLISHED",
]
```
## DateComparisonTypeType

```python
# DateComparisonTypeType usage example
from types_aiobotocore_connect.literals import DateComparisonTypeType

def get_value() -> DateComparisonTypeType:
    return "EQUAL_TO"
```

```python
# DateComparisonTypeType definition
DateComparisonTypeType = Literal[
    "EQUAL_TO",
    "GREATER_THAN",
    "GREATER_THAN_OR_EQUAL_TO",
    "LESS_THAN",
    "LESS_THAN_OR_EQUAL_TO",
]
```
## DateTimeComparisonTypeType

```python
# DateTimeComparisonTypeType usage example
from types_aiobotocore_connect.literals import DateTimeComparisonTypeType

def get_value() -> DateTimeComparisonTypeType:
    return "EQUAL_TO"
```

```python
# DateTimeComparisonTypeType definition
DateTimeComparisonTypeType = Literal[
    "EQUAL_TO",
    "GREATER_THAN",
    "GREATER_THAN_OR_EQUAL_TO",
    "LESS_THAN",
    "LESS_THAN_OR_EQUAL_TO",
    "RANGE",
]
```
## DecimalComparisonTypeType

```python
# DecimalComparisonTypeType usage example
from types_aiobotocore_connect.literals import DecimalComparisonTypeType

def get_value() -> DecimalComparisonTypeType:
    return "EQUAL"
```

```python
# DecimalComparisonTypeType definition
DecimalComparisonTypeType = Literal[
    "EQUAL",
    "GREATER",
    "GREATER_OR_EQUAL",
    "LESSER",
    "LESSER_OR_EQUAL",
    "NOT_EQUAL",
    "RANGE",
]
```
## DeviceTypeType

```python
# DeviceTypeType usage example
from types_aiobotocore_connect.literals import DeviceTypeType

def get_value() -> DeviceTypeType:
    return "APNS"
```

```python
# DeviceTypeType definition
DeviceTypeType = Literal[
    "APNS",
    "APNS_SANDBOX",
    "GCM",
]
```
## DirectoryTypeType

```python
# DirectoryTypeType usage example
from types_aiobotocore_connect.literals import DirectoryTypeType

def get_value() -> DirectoryTypeType:
    return "CONNECT_MANAGED"
```

```python
# DirectoryTypeType definition
DirectoryTypeType = Literal[
    "CONNECT_MANAGED",
    "EXISTING_DIRECTORY",
    "SAML",
]
```
## DisconnectOnCustomerExitParticipantTypeType

```python
# DisconnectOnCustomerExitParticipantTypeType usage example
from types_aiobotocore_connect.literals import DisconnectOnCustomerExitParticipantTypeType

def get_value() -> DisconnectOnCustomerExitParticipantTypeType:
    return "AGENT"
```

```python
# DisconnectOnCustomerExitParticipantTypeType definition
DisconnectOnCustomerExitParticipantTypeType = Literal[
    "AGENT",
]
```
## EmailHeaderTypeType

```python
# EmailHeaderTypeType usage example
from types_aiobotocore_connect.literals import EmailHeaderTypeType

def get_value() -> EmailHeaderTypeType:
    return "IN_REPLY_TO"
```

```python
# EmailHeaderTypeType definition
EmailHeaderTypeType = Literal[
    "IN_REPLY_TO",
    "MESSAGE_ID",
    "REFERENCES",
    "X_SES_SPAM_VERDICT",
    "X_SES_VIRUS_VERDICT",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example
from types_aiobotocore_connect.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "KMS"
```

```python
# EncryptionTypeType definition
EncryptionTypeType = Literal[
    "KMS",
]
```
## EndpointTypeType

```python
# EndpointTypeType usage example
from types_aiobotocore_connect.literals import EndpointTypeType

def get_value() -> EndpointTypeType:
    return "CONNECT_PHONENUMBER_ARN"
```

```python
# EndpointTypeType definition
EndpointTypeType = Literal[
    "CONNECT_PHONENUMBER_ARN",
    "CONTACT_FLOW",
    "EMAIL_ADDRESS",
    "TELEPHONE_NUMBER",
    "VOIP",
]
```
## EntityTypeType

```python
# EntityTypeType usage example
from types_aiobotocore_connect.literals import EntityTypeType

def get_value() -> EntityTypeType:
    return "AI_AGENT"
```

```python
# EntityTypeType definition
EntityTypeType = Literal[
    "AI_AGENT",
    "USER",
]
```
## EvaluationFormItemEnablementActionType

```python
# EvaluationFormItemEnablementActionType usage example
from types_aiobotocore_connect.literals import EvaluationFormItemEnablementActionType

def get_value() -> EvaluationFormItemEnablementActionType:
    return "DISABLE"
```

```python
# EvaluationFormItemEnablementActionType definition
EvaluationFormItemEnablementActionType = Literal[
    "DISABLE",
    "ENABLE",
]
```
## EvaluationFormItemEnablementOperatorType

```python
# EvaluationFormItemEnablementOperatorType usage example
from types_aiobotocore_connect.literals import EvaluationFormItemEnablementOperatorType

def get_value() -> EvaluationFormItemEnablementOperatorType:
    return "AND"
```

```python
# EvaluationFormItemEnablementOperatorType definition
EvaluationFormItemEnablementOperatorType = Literal[
    "AND",
    "OR",
]
```
## EvaluationFormItemEnablementSourceTypeType

```python
# EvaluationFormItemEnablementSourceTypeType usage example
from types_aiobotocore_connect.literals import EvaluationFormItemEnablementSourceTypeType

def get_value() -> EvaluationFormItemEnablementSourceTypeType:
    return "QUESTION_REF_ID"
```

```python
# EvaluationFormItemEnablementSourceTypeType definition
EvaluationFormItemEnablementSourceTypeType = Literal[
    "QUESTION_REF_ID",
]
```
## EvaluationFormItemEnablementSourceValueTypeType

```python
# EvaluationFormItemEnablementSourceValueTypeType usage example
from types_aiobotocore_connect.literals import EvaluationFormItemEnablementSourceValueTypeType

def get_value() -> EvaluationFormItemEnablementSourceValueTypeType:
    return "OPTION_REF_ID"
```

```python
# EvaluationFormItemEnablementSourceValueTypeType definition
EvaluationFormItemEnablementSourceValueTypeType = Literal[
    "OPTION_REF_ID",
]
```
## EvaluationFormItemSourceValuesComparatorType

```python
# EvaluationFormItemSourceValuesComparatorType usage example
from types_aiobotocore_connect.literals import EvaluationFormItemSourceValuesComparatorType

def get_value() -> EvaluationFormItemSourceValuesComparatorType:
    return "ALL_IN"
```

```python
# EvaluationFormItemSourceValuesComparatorType definition
EvaluationFormItemSourceValuesComparatorType = Literal[
    "ALL_IN",
    "EXACT",
    "IN",
    "NOT_IN",
]
```
## EvaluationFormLanguageCodeType

```python
# EvaluationFormLanguageCodeType usage example
from types_aiobotocore_connect.literals import EvaluationFormLanguageCodeType

def get_value() -> EvaluationFormLanguageCodeType:
    return "de-DE"
```

```python
# EvaluationFormLanguageCodeType definition
EvaluationFormLanguageCodeType = Literal[
    "de-DE",
    "en-US",
    "es-ES",
    "fr-FR",
    "it-IT",
    "pt-BR",
]
```
## EvaluationFormMultiSelectQuestionDisplayModeType

```python
# EvaluationFormMultiSelectQuestionDisplayModeType usage example
from types_aiobotocore_connect.literals import EvaluationFormMultiSelectQuestionDisplayModeType

def get_value() -> EvaluationFormMultiSelectQuestionDisplayModeType:
    return "CHECKBOX"
```

```python
# EvaluationFormMultiSelectQuestionDisplayModeType definition
EvaluationFormMultiSelectQuestionDisplayModeType = Literal[
    "CHECKBOX",
    "DROPDOWN",
]
```
## EvaluationFormQuestionAutomationAnswerSourceTypeType

```python
# EvaluationFormQuestionAutomationAnswerSourceTypeType usage example
from types_aiobotocore_connect.literals import EvaluationFormQuestionAutomationAnswerSourceTypeType

def get_value() -> EvaluationFormQuestionAutomationAnswerSourceTypeType:
    return "CONTACT_LENS_DATA"
```

```python
# EvaluationFormQuestionAutomationAnswerSourceTypeType definition
EvaluationFormQuestionAutomationAnswerSourceTypeType = Literal[
    "CONTACT_LENS_DATA",
    "GEN_AI",
]
```
## EvaluationFormQuestionTypeType

```python
# EvaluationFormQuestionTypeType usage example
from types_aiobotocore_connect.literals import EvaluationFormQuestionTypeType

def get_value() -> EvaluationFormQuestionTypeType:
    return "DATETIME"
```

```python
# EvaluationFormQuestionTypeType definition
EvaluationFormQuestionTypeType = Literal[
    "DATETIME",
    "MULTISELECT",
    "NUMERIC",
    "SINGLESELECT",
    "TEXT",
]
```
## EvaluationFormScoringModeType

```python
# EvaluationFormScoringModeType usage example
from types_aiobotocore_connect.literals import EvaluationFormScoringModeType

def get_value() -> EvaluationFormScoringModeType:
    return "QUESTION_ONLY"
```

```python
# EvaluationFormScoringModeType definition
EvaluationFormScoringModeType = Literal[
    "QUESTION_ONLY",
    "SECTION_ONLY",
]
```
## EvaluationFormScoringStatusType

```python
# EvaluationFormScoringStatusType usage example
from types_aiobotocore_connect.literals import EvaluationFormScoringStatusType

def get_value() -> EvaluationFormScoringStatusType:
    return "DISABLED"
```

```python
# EvaluationFormScoringStatusType definition
EvaluationFormScoringStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EvaluationFormSingleSelectQuestionDisplayModeType

```python
# EvaluationFormSingleSelectQuestionDisplayModeType usage example
from types_aiobotocore_connect.literals import EvaluationFormSingleSelectQuestionDisplayModeType

def get_value() -> EvaluationFormSingleSelectQuestionDisplayModeType:
    return "DROPDOWN"
```

```python
# EvaluationFormSingleSelectQuestionDisplayModeType definition
EvaluationFormSingleSelectQuestionDisplayModeType = Literal[
    "DROPDOWN",
    "RADIO",
]
```
## EvaluationFormVersionStatusType

```python
# EvaluationFormVersionStatusType usage example
from types_aiobotocore_connect.literals import EvaluationFormVersionStatusType

def get_value() -> EvaluationFormVersionStatusType:
    return "ACTIVE"
```

```python
# EvaluationFormVersionStatusType definition
EvaluationFormVersionStatusType = Literal[
    "ACTIVE",
    "DRAFT",
]
```
## EvaluationQuestionAnswerAnalysisTypeType

```python
# EvaluationQuestionAnswerAnalysisTypeType usage example
from types_aiobotocore_connect.literals import EvaluationQuestionAnswerAnalysisTypeType

def get_value() -> EvaluationQuestionAnswerAnalysisTypeType:
    return "CONTACT_LENS_DATA"
```

```python
# EvaluationQuestionAnswerAnalysisTypeType definition
EvaluationQuestionAnswerAnalysisTypeType = Literal[
    "CONTACT_LENS_DATA",
    "GEN_AI",
]
```
## EvaluationReviewNotificationRecipientTypeType

```python
# EvaluationReviewNotificationRecipientTypeType usage example
from types_aiobotocore_connect.literals import EvaluationReviewNotificationRecipientTypeType

def get_value() -> EvaluationReviewNotificationRecipientTypeType:
    return "USER_ID"
```

```python
# EvaluationReviewNotificationRecipientTypeType definition
EvaluationReviewNotificationRecipientTypeType = Literal[
    "USER_ID",
]
```
## EvaluationStatusType

```python
# EvaluationStatusType usage example
from types_aiobotocore_connect.literals import EvaluationStatusType

def get_value() -> EvaluationStatusType:
    return "DRAFT"
```

```python
# EvaluationStatusType definition
EvaluationStatusType = Literal[
    "DRAFT",
    "REVIEW_REQUESTED",
    "SUBMITTED",
    "UNDER_REVIEW",
]
```
## EvaluationSuggestedAnswerStatusType

```python
# EvaluationSuggestedAnswerStatusType usage example
from types_aiobotocore_connect.literals import EvaluationSuggestedAnswerStatusType

def get_value() -> EvaluationSuggestedAnswerStatusType:
    return "FAILED"
```

```python
# EvaluationSuggestedAnswerStatusType definition
EvaluationSuggestedAnswerStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCEEDED",
]
```
## EvaluationTranscriptTypeType

```python
# EvaluationTranscriptTypeType usage example
from types_aiobotocore_connect.literals import EvaluationTranscriptTypeType

def get_value() -> EvaluationTranscriptTypeType:
    return "RAW"
```

```python
# EvaluationTranscriptTypeType definition
EvaluationTranscriptTypeType = Literal[
    "RAW",
    "REDACTED",
]
```
## EvaluationTypeType

```python
# EvaluationTypeType usage example
from types_aiobotocore_connect.literals import EvaluationTypeType

def get_value() -> EvaluationTypeType:
    return "CALIBRATION"
```

```python
# EvaluationTypeType definition
EvaluationTypeType = Literal[
    "CALIBRATION",
    "STANDARD",
]
```
## EventSourceNameType

```python
# EventSourceNameType usage example
from types_aiobotocore_connect.literals import EventSourceNameType

def get_value() -> EventSourceNameType:
    return "OnCaseCreate"
```

```python
# EventSourceNameType definition
EventSourceNameType = Literal[
    "OnCaseCreate",
    "OnCaseUpdate",
    "OnContactEvaluationSubmit",
    "OnMetricDataUpdate",
    "OnPostCallAnalysisAvailable",
    "OnPostChatAnalysisAvailable",
    "OnRealTimeCallAnalysisAvailable",
    "OnRealTimeChatAnalysisAvailable",
    "OnSalesforceCaseCreate",
    "OnSlaBreach",
    "OnZendeskTicketCreate",
    "OnZendeskTicketStatusUpdate",
]
```
## FailureReasonCodeType

```python
# FailureReasonCodeType usage example
from types_aiobotocore_connect.literals import FailureReasonCodeType

def get_value() -> FailureReasonCodeType:
    return "IDEMPOTENCY_EXCEPTION"
```

```python
# FailureReasonCodeType definition
FailureReasonCodeType = Literal[
    "IDEMPOTENCY_EXCEPTION",
    "INTERNAL_ERROR",
    "INVALID_ATTRIBUTE_KEY",
    "INVALID_CUSTOMER_ENDPOINT",
    "INVALID_OUTBOUND_STRATEGY",
    "INVALID_QUEUE",
    "INVALID_SYSTEM_ENDPOINT",
    "MISSING_CAMPAIGN",
    "MISSING_CUSTOMER_ENDPOINT",
    "MISSING_QUEUE_ID_AND_SYSTEM_ENDPOINT",
    "REQUEST_THROTTLED",
]
```
## FileStatusTypeType

```python
# FileStatusTypeType usage example
from types_aiobotocore_connect.literals import FileStatusTypeType

def get_value() -> FileStatusTypeType:
    return "APPROVED"
```

```python
# FileStatusTypeType definition
FileStatusTypeType = Literal[
    "APPROVED",
    "FAILED",
    "PROCESSING",
    "REJECTED",
]
```
## FileUseCaseTypeType

```python
# FileUseCaseTypeType usage example
from types_aiobotocore_connect.literals import FileUseCaseTypeType

def get_value() -> FileUseCaseTypeType:
    return "ATTACHMENT"
```

```python
# FileUseCaseTypeType definition
FileUseCaseTypeType = Literal[
    "ATTACHMENT",
    "EMAIL_MESSAGE",
]
```
## FilterV2StringConditionComparisonOperatorType

```python
# FilterV2StringConditionComparisonOperatorType usage example
from types_aiobotocore_connect.literals import FilterV2StringConditionComparisonOperatorType

def get_value() -> FilterV2StringConditionComparisonOperatorType:
    return "NOT_EXISTS"
```

```python
# FilterV2StringConditionComparisonOperatorType definition
FilterV2StringConditionComparisonOperatorType = Literal[
    "NOT_EXISTS",
]
```
## FlowAssociationResourceTypeType

```python
# FlowAssociationResourceTypeType usage example
from types_aiobotocore_connect.literals import FlowAssociationResourceTypeType

def get_value() -> FlowAssociationResourceTypeType:
    return "ANALYTICS_CONNECTOR"
```

```python
# FlowAssociationResourceTypeType definition
FlowAssociationResourceTypeType = Literal[
    "ANALYTICS_CONNECTOR",
    "INBOUND_EMAIL",
    "OUTBOUND_EMAIL",
    "SMS_PHONE_NUMBER",
    "WHATSAPP_MESSAGING_PHONE_NUMBER",
]
```
## FlowModuleTypeType

```python
# FlowModuleTypeType usage example
from types_aiobotocore_connect.literals import FlowModuleTypeType

def get_value() -> FlowModuleTypeType:
    return "MCP"
```

```python
# FlowModuleTypeType definition
FlowModuleTypeType = Literal[
    "MCP",
]
```
## GetMetricDataPaginatorName

```python
# GetMetricDataPaginatorName usage example
from types_aiobotocore_connect.literals import GetMetricDataPaginatorName

def get_value() -> GetMetricDataPaginatorName:
    return "get_metric_data"
```

```python
# GetMetricDataPaginatorName definition
GetMetricDataPaginatorName = Literal[
    "get_metric_data",
]
```
## GroupingType

```python
# GroupingType usage example
from types_aiobotocore_connect.literals import GroupingType

def get_value() -> GroupingType:
    return "AGENT_STATUS"
```

```python
# GroupingType definition
GroupingType = Literal[
    "AGENT_STATUS",
    "CHANNEL",
    "QUEUE",
    "ROUTING_PROFILE",
    "ROUTING_STEP_EXPRESSION",
    "SUBTYPE",
    "VALIDATION_TEST_TYPE",
]
```
## HierarchyGroupMatchTypeType

```python
# HierarchyGroupMatchTypeType usage example
from types_aiobotocore_connect.literals import HierarchyGroupMatchTypeType

def get_value() -> HierarchyGroupMatchTypeType:
    return "EXACT"
```

```python
# HierarchyGroupMatchTypeType definition
HierarchyGroupMatchTypeType = Literal[
    "EXACT",
    "WITH_CHILD_GROUPS",
]
```
## HistoricalMetricNameType

```python
# HistoricalMetricNameType usage example
from types_aiobotocore_connect.literals import HistoricalMetricNameType

def get_value() -> HistoricalMetricNameType:
    return "ABANDON_TIME"
```

```python
# HistoricalMetricNameType definition
HistoricalMetricNameType = Literal[
    "ABANDON_TIME",
    "AFTER_CONTACT_WORK_TIME",
    "API_CONTACTS_HANDLED",
    "CALLBACK_CONTACTS_HANDLED",
    "CONTACTS_ABANDONED",
    "CONTACTS_AGENT_HUNG_UP_FIRST",
    "CONTACTS_CONSULTED",
    "CONTACTS_HANDLED",
    "CONTACTS_HANDLED_INCOMING",
    "CONTACTS_HANDLED_OUTBOUND",
    "CONTACTS_HOLD_ABANDONS",
    "CONTACTS_MISSED",
    "CONTACTS_QUEUED",
    "CONTACTS_TRANSFERRED_IN",
    "CONTACTS_TRANSFERRED_IN_FROM_QUEUE",
    "CONTACTS_TRANSFERRED_OUT",
    "CONTACTS_TRANSFERRED_OUT_FROM_QUEUE",
    "HANDLE_TIME",
    "HOLD_TIME",
    "INTERACTION_AND_HOLD_TIME",
    "INTERACTION_TIME",
    "OCCUPANCY",
    "QUEUE_ANSWER_TIME",
    "QUEUED_TIME",
    "SERVICE_LEVEL",
]
```
## HoursOfOperationDaysType

```python
# HoursOfOperationDaysType usage example
from types_aiobotocore_connect.literals import HoursOfOperationDaysType

def get_value() -> HoursOfOperationDaysType:
    return "FRIDAY"
```

```python
# HoursOfOperationDaysType definition
HoursOfOperationDaysType = Literal[
    "FRIDAY",
    "MONDAY",
    "SATURDAY",
    "SUNDAY",
    "THURSDAY",
    "TUESDAY",
    "WEDNESDAY",
]
```
## InboundMessageSourceTypeType

```python
# InboundMessageSourceTypeType usage example
from types_aiobotocore_connect.literals import InboundMessageSourceTypeType

def get_value() -> InboundMessageSourceTypeType:
    return "RAW"
```

```python
# InboundMessageSourceTypeType definition
InboundMessageSourceTypeType = Literal[
    "RAW",
]
```
## InitiateAsType

```python
# InitiateAsType usage example
from types_aiobotocore_connect.literals import InitiateAsType

def get_value() -> InitiateAsType:
    return "COMPLETED"
```

```python
# InitiateAsType definition
InitiateAsType = Literal[
    "COMPLETED",
    "CONNECTED_TO_USER",
]
```
## InstanceAttributeTypeType

```python
# InstanceAttributeTypeType usage example
from types_aiobotocore_connect.literals import InstanceAttributeTypeType

def get_value() -> InstanceAttributeTypeType:
    return "AUTO_RESOLVE_BEST_VOICES"
```

```python
# InstanceAttributeTypeType definition
InstanceAttributeTypeType = Literal[
    "AUTO_RESOLVE_BEST_VOICES",
    "CONTACT_LENS",
    "CONTACTFLOW_LOGS",
    "EARLY_MEDIA",
    "ENHANCED_CHAT_MONITORING",
    "ENHANCED_CONTACT_MONITORING",
    "HIGH_VOLUME_OUTBOUND",
    "INBOUND_CALLS",
    "MESSAGE_STREAMING",
    "MULTI_PARTY_CHAT_CONFERENCE",
    "MULTI_PARTY_CONFERENCE",
    "OUTBOUND_CALLS",
    "USE_CUSTOM_TTS_VOICES",
]
```
## InstanceReplicationStatusType

```python
# InstanceReplicationStatusType usage example
from types_aiobotocore_connect.literals import InstanceReplicationStatusType

def get_value() -> InstanceReplicationStatusType:
    return "INSTANCE_REPLICATION_COMPLETE"
```

```python
# InstanceReplicationStatusType definition
InstanceReplicationStatusType = Literal[
    "INSTANCE_REPLICA_DELETING",
    "INSTANCE_REPLICATION_COMPLETE",
    "INSTANCE_REPLICATION_DELETION_FAILED",
    "INSTANCE_REPLICATION_FAILED",
    "INSTANCE_REPLICATION_IN_PROGRESS",
    "RESOURCE_REPLICATION_NOT_STARTED",
]
```
## InstanceStatusType

```python
# InstanceStatusType usage example
from types_aiobotocore_connect.literals import InstanceStatusType

def get_value() -> InstanceStatusType:
    return "ACTIVE"
```

```python
# InstanceStatusType definition
InstanceStatusType = Literal[
    "ACTIVE",
    "CREATION_FAILED",
    "CREATION_IN_PROGRESS",
]
```
## InstanceStorageResourceTypeType

```python
# InstanceStorageResourceTypeType usage example
from types_aiobotocore_connect.literals import InstanceStorageResourceTypeType

def get_value() -> InstanceStorageResourceTypeType:
    return "AGENT_EVENTS"
```

```python
# InstanceStorageResourceTypeType definition
InstanceStorageResourceTypeType = Literal[
    "AGENT_EVENTS",
    "ATTACHMENTS",
    "CALL_RECORDINGS",
    "CHAT_TRANSCRIPTS",
    "CONTACT_EVALUATIONS",
    "CONTACT_TRACE_RECORDS",
    "EMAIL_MESSAGES",
    "MEDIA_STREAMS",
    "REAL_TIME_CONTACT_ANALYSIS_CHAT_SEGMENTS",
    "REAL_TIME_CONTACT_ANALYSIS_SEGMENTS",
    "REAL_TIME_CONTACT_ANALYSIS_VOICE_SEGMENTS",
    "SCHEDULED_REPORTS",
    "SCREEN_RECORDINGS",
]
```
## IntegrationTypeType

```python
# IntegrationTypeType usage example
from types_aiobotocore_connect.literals import IntegrationTypeType

def get_value() -> IntegrationTypeType:
    return "ANALYTICS_CONNECTOR"
```

```python
# IntegrationTypeType definition
IntegrationTypeType = Literal[
    "ANALYTICS_CONNECTOR",
    "APPLICATION",
    "CALL_TRANSFER_CONNECTOR",
    "CASES_DOMAIN",
    "COGNITO_USER_POOL",
    "EVENT",
    "FILE_SCANNER",
    "MESSAGE_PROCESSOR",
    "PINPOINT_APP",
    "Q_MESSAGE_TEMPLATES",
    "SES_IDENTITY",
    "VOICE_ID",
    "WISDOM_ASSISTANT",
    "WISDOM_KNOWLEDGE_BASE",
    "WISDOM_QUICK_RESPONSES",
]
```
## IntervalPeriodType

```python
# IntervalPeriodType usage example
from types_aiobotocore_connect.literals import IntervalPeriodType

def get_value() -> IntervalPeriodType:
    return "DAY"
```

```python
# IntervalPeriodType definition
IntervalPeriodType = Literal[
    "DAY",
    "FIFTEEN_MIN",
    "HOUR",
    "THIRTY_MIN",
    "TOTAL",
    "WEEK",
]
```
## IvrRecordingTrackType

```python
# IvrRecordingTrackType usage example
from types_aiobotocore_connect.literals import IvrRecordingTrackType

def get_value() -> IvrRecordingTrackType:
    return "ALL"
```

```python
# IvrRecordingTrackType definition
IvrRecordingTrackType = Literal[
    "ALL",
]
```
## LexVersionType

```python
# LexVersionType usage example
from types_aiobotocore_connect.literals import LexVersionType

def get_value() -> LexVersionType:
    return "V1"
```

```python
# LexVersionType definition
LexVersionType = Literal[
    "V1",
    "V2",
]
```
## ListAgentStatusesPaginatorName

```python
# ListAgentStatusesPaginatorName usage example
from types_aiobotocore_connect.literals import ListAgentStatusesPaginatorName

def get_value() -> ListAgentStatusesPaginatorName:
    return "list_agent_statuses"
```

```python
# ListAgentStatusesPaginatorName definition
ListAgentStatusesPaginatorName = Literal[
    "list_agent_statuses",
]
```
## ListApprovedOriginsPaginatorName

```python
# ListApprovedOriginsPaginatorName usage example
from types_aiobotocore_connect.literals import ListApprovedOriginsPaginatorName

def get_value() -> ListApprovedOriginsPaginatorName:
    return "list_approved_origins"
```

```python
# ListApprovedOriginsPaginatorName definition
ListApprovedOriginsPaginatorName = Literal[
    "list_approved_origins",
]
```
## ListAuthenticationProfilesPaginatorName

```python
# ListAuthenticationProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import ListAuthenticationProfilesPaginatorName

def get_value() -> ListAuthenticationProfilesPaginatorName:
    return "list_authentication_profiles"
```

```python
# ListAuthenticationProfilesPaginatorName definition
ListAuthenticationProfilesPaginatorName = Literal[
    "list_authentication_profiles",
]
```
## ListBotsPaginatorName

```python
# ListBotsPaginatorName usage example
from types_aiobotocore_connect.literals import ListBotsPaginatorName

def get_value() -> ListBotsPaginatorName:
    return "list_bots"
```

```python
# ListBotsPaginatorName definition
ListBotsPaginatorName = Literal[
    "list_bots",
]
```
## ListChildHoursOfOperationsPaginatorName

```python
# ListChildHoursOfOperationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListChildHoursOfOperationsPaginatorName

def get_value() -> ListChildHoursOfOperationsPaginatorName:
    return "list_child_hours_of_operations"
```

```python
# ListChildHoursOfOperationsPaginatorName definition
ListChildHoursOfOperationsPaginatorName = Literal[
    "list_child_hours_of_operations",
]
```
## ListContactEvaluationsPaginatorName

```python
# ListContactEvaluationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactEvaluationsPaginatorName

def get_value() -> ListContactEvaluationsPaginatorName:
    return "list_contact_evaluations"
```

```python
# ListContactEvaluationsPaginatorName definition
ListContactEvaluationsPaginatorName = Literal[
    "list_contact_evaluations",
]
```
## ListContactFlowModuleAliasesPaginatorName

```python
# ListContactFlowModuleAliasesPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactFlowModuleAliasesPaginatorName

def get_value() -> ListContactFlowModuleAliasesPaginatorName:
    return "list_contact_flow_module_aliases"
```

```python
# ListContactFlowModuleAliasesPaginatorName definition
ListContactFlowModuleAliasesPaginatorName = Literal[
    "list_contact_flow_module_aliases",
]
```
## ListContactFlowModuleVersionsPaginatorName

```python
# ListContactFlowModuleVersionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactFlowModuleVersionsPaginatorName

def get_value() -> ListContactFlowModuleVersionsPaginatorName:
    return "list_contact_flow_module_versions"
```

```python
# ListContactFlowModuleVersionsPaginatorName definition
ListContactFlowModuleVersionsPaginatorName = Literal[
    "list_contact_flow_module_versions",
]
```
## ListContactFlowModulesPaginatorName

```python
# ListContactFlowModulesPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactFlowModulesPaginatorName

def get_value() -> ListContactFlowModulesPaginatorName:
    return "list_contact_flow_modules"
```

```python
# ListContactFlowModulesPaginatorName definition
ListContactFlowModulesPaginatorName = Literal[
    "list_contact_flow_modules",
]
```
## ListContactFlowVersionsPaginatorName

```python
# ListContactFlowVersionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactFlowVersionsPaginatorName

def get_value() -> ListContactFlowVersionsPaginatorName:
    return "list_contact_flow_versions"
```

```python
# ListContactFlowVersionsPaginatorName definition
ListContactFlowVersionsPaginatorName = Literal[
    "list_contact_flow_versions",
]
```
## ListContactFlowsPaginatorName

```python
# ListContactFlowsPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactFlowsPaginatorName

def get_value() -> ListContactFlowsPaginatorName:
    return "list_contact_flows"
```

```python
# ListContactFlowsPaginatorName definition
ListContactFlowsPaginatorName = Literal[
    "list_contact_flows",
]
```
## ListContactReferencesPaginatorName

```python
# ListContactReferencesPaginatorName usage example
from types_aiobotocore_connect.literals import ListContactReferencesPaginatorName

def get_value() -> ListContactReferencesPaginatorName:
    return "list_contact_references"
```

```python
# ListContactReferencesPaginatorName definition
ListContactReferencesPaginatorName = Literal[
    "list_contact_references",
]
```
## ListDataTableAttributesPaginatorName

```python
# ListDataTableAttributesPaginatorName usage example
from types_aiobotocore_connect.literals import ListDataTableAttributesPaginatorName

def get_value() -> ListDataTableAttributesPaginatorName:
    return "list_data_table_attributes"
```

```python
# ListDataTableAttributesPaginatorName definition
ListDataTableAttributesPaginatorName = Literal[
    "list_data_table_attributes",
]
```
## ListDataTablePrimaryValuesPaginatorName

```python
# ListDataTablePrimaryValuesPaginatorName usage example
from types_aiobotocore_connect.literals import ListDataTablePrimaryValuesPaginatorName

def get_value() -> ListDataTablePrimaryValuesPaginatorName:
    return "list_data_table_primary_values"
```

```python
# ListDataTablePrimaryValuesPaginatorName definition
ListDataTablePrimaryValuesPaginatorName = Literal[
    "list_data_table_primary_values",
]
```
## ListDataTableValuesPaginatorName

```python
# ListDataTableValuesPaginatorName usage example
from types_aiobotocore_connect.literals import ListDataTableValuesPaginatorName

def get_value() -> ListDataTableValuesPaginatorName:
    return "list_data_table_values"
```

```python
# ListDataTableValuesPaginatorName definition
ListDataTableValuesPaginatorName = Literal[
    "list_data_table_values",
]
```
## ListDataTablesPaginatorName

```python
# ListDataTablesPaginatorName usage example
from types_aiobotocore_connect.literals import ListDataTablesPaginatorName

def get_value() -> ListDataTablesPaginatorName:
    return "list_data_tables"
```

```python
# ListDataTablesPaginatorName definition
ListDataTablesPaginatorName = Literal[
    "list_data_tables",
]
```
## ListDefaultVocabulariesPaginatorName

```python
# ListDefaultVocabulariesPaginatorName usage example
from types_aiobotocore_connect.literals import ListDefaultVocabulariesPaginatorName

def get_value() -> ListDefaultVocabulariesPaginatorName:
    return "list_default_vocabularies"
```

```python
# ListDefaultVocabulariesPaginatorName definition
ListDefaultVocabulariesPaginatorName = Literal[
    "list_default_vocabularies",
]
```
## ListEntitySecurityProfilesPaginatorName

```python
# ListEntitySecurityProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import ListEntitySecurityProfilesPaginatorName

def get_value() -> ListEntitySecurityProfilesPaginatorName:
    return "list_entity_security_profiles"
```

```python
# ListEntitySecurityProfilesPaginatorName definition
ListEntitySecurityProfilesPaginatorName = Literal[
    "list_entity_security_profiles",
]
```
## ListEvaluationFormVersionsPaginatorName

```python
# ListEvaluationFormVersionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListEvaluationFormVersionsPaginatorName

def get_value() -> ListEvaluationFormVersionsPaginatorName:
    return "list_evaluation_form_versions"
```

```python
# ListEvaluationFormVersionsPaginatorName definition
ListEvaluationFormVersionsPaginatorName = Literal[
    "list_evaluation_form_versions",
]
```
## ListEvaluationFormsPaginatorName

```python
# ListEvaluationFormsPaginatorName usage example
from types_aiobotocore_connect.literals import ListEvaluationFormsPaginatorName

def get_value() -> ListEvaluationFormsPaginatorName:
    return "list_evaluation_forms"
```

```python
# ListEvaluationFormsPaginatorName definition
ListEvaluationFormsPaginatorName = Literal[
    "list_evaluation_forms",
]
```
## ListFlowAssociationResourceTypeType

```python
# ListFlowAssociationResourceTypeType usage example
from types_aiobotocore_connect.literals import ListFlowAssociationResourceTypeType

def get_value() -> ListFlowAssociationResourceTypeType:
    return "ANALYTICS_CONNECTOR"
```

```python
# ListFlowAssociationResourceTypeType definition
ListFlowAssociationResourceTypeType = Literal[
    "ANALYTICS_CONNECTOR",
    "INBOUND_EMAIL",
    "OUTBOUND_EMAIL",
    "VOICE_PHONE_NUMBER",
    "WHATSAPP_MESSAGING_PHONE_NUMBER",
]
```
## ListFlowAssociationsPaginatorName

```python
# ListFlowAssociationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListFlowAssociationsPaginatorName

def get_value() -> ListFlowAssociationsPaginatorName:
    return "list_flow_associations"
```

```python
# ListFlowAssociationsPaginatorName definition
ListFlowAssociationsPaginatorName = Literal[
    "list_flow_associations",
]
```
## ListHoursOfOperationOverridesPaginatorName

```python
# ListHoursOfOperationOverridesPaginatorName usage example
from types_aiobotocore_connect.literals import ListHoursOfOperationOverridesPaginatorName

def get_value() -> ListHoursOfOperationOverridesPaginatorName:
    return "list_hours_of_operation_overrides"
```

```python
# ListHoursOfOperationOverridesPaginatorName definition
ListHoursOfOperationOverridesPaginatorName = Literal[
    "list_hours_of_operation_overrides",
]
```
## ListHoursOfOperationsPaginatorName

```python
# ListHoursOfOperationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListHoursOfOperationsPaginatorName

def get_value() -> ListHoursOfOperationsPaginatorName:
    return "list_hours_of_operations"
```

```python
# ListHoursOfOperationsPaginatorName definition
ListHoursOfOperationsPaginatorName = Literal[
    "list_hours_of_operations",
]
```
## ListInstanceAttributesPaginatorName

```python
# ListInstanceAttributesPaginatorName usage example
from types_aiobotocore_connect.literals import ListInstanceAttributesPaginatorName

def get_value() -> ListInstanceAttributesPaginatorName:
    return "list_instance_attributes"
```

```python
# ListInstanceAttributesPaginatorName definition
ListInstanceAttributesPaginatorName = Literal[
    "list_instance_attributes",
]
```
## ListInstanceStorageConfigsPaginatorName

```python
# ListInstanceStorageConfigsPaginatorName usage example
from types_aiobotocore_connect.literals import ListInstanceStorageConfigsPaginatorName

def get_value() -> ListInstanceStorageConfigsPaginatorName:
    return "list_instance_storage_configs"
```

```python
# ListInstanceStorageConfigsPaginatorName definition
ListInstanceStorageConfigsPaginatorName = Literal[
    "list_instance_storage_configs",
]
```
## ListInstancesPaginatorName

```python
# ListInstancesPaginatorName usage example
from types_aiobotocore_connect.literals import ListInstancesPaginatorName

def get_value() -> ListInstancesPaginatorName:
    return "list_instances"
```

```python
# ListInstancesPaginatorName definition
ListInstancesPaginatorName = Literal[
    "list_instances",
]
```
## ListIntegrationAssociationsPaginatorName

```python
# ListIntegrationAssociationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListIntegrationAssociationsPaginatorName

def get_value() -> ListIntegrationAssociationsPaginatorName:
    return "list_integration_associations"
```

```python
# ListIntegrationAssociationsPaginatorName definition
ListIntegrationAssociationsPaginatorName = Literal[
    "list_integration_associations",
]
```
## ListLambdaFunctionsPaginatorName

```python
# ListLambdaFunctionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListLambdaFunctionsPaginatorName

def get_value() -> ListLambdaFunctionsPaginatorName:
    return "list_lambda_functions"
```

```python
# ListLambdaFunctionsPaginatorName definition
ListLambdaFunctionsPaginatorName = Literal[
    "list_lambda_functions",
]
```
## ListLexBotsPaginatorName

```python
# ListLexBotsPaginatorName usage example
from types_aiobotocore_connect.literals import ListLexBotsPaginatorName

def get_value() -> ListLexBotsPaginatorName:
    return "list_lex_bots"
```

```python
# ListLexBotsPaginatorName definition
ListLexBotsPaginatorName = Literal[
    "list_lex_bots",
]
```
## ListPhoneNumbersPaginatorName

```python
# ListPhoneNumbersPaginatorName usage example
from types_aiobotocore_connect.literals import ListPhoneNumbersPaginatorName

def get_value() -> ListPhoneNumbersPaginatorName:
    return "list_phone_numbers"
```

```python
# ListPhoneNumbersPaginatorName definition
ListPhoneNumbersPaginatorName = Literal[
    "list_phone_numbers",
]
```
## ListPhoneNumbersV2PaginatorName

```python
# ListPhoneNumbersV2PaginatorName usage example
from types_aiobotocore_connect.literals import ListPhoneNumbersV2PaginatorName

def get_value() -> ListPhoneNumbersV2PaginatorName:
    return "list_phone_numbers_v2"
```

```python
# ListPhoneNumbersV2PaginatorName definition
ListPhoneNumbersV2PaginatorName = Literal[
    "list_phone_numbers_v2",
]
```
## ListPredefinedAttributesPaginatorName

```python
# ListPredefinedAttributesPaginatorName usage example
from types_aiobotocore_connect.literals import ListPredefinedAttributesPaginatorName

def get_value() -> ListPredefinedAttributesPaginatorName:
    return "list_predefined_attributes"
```

```python
# ListPredefinedAttributesPaginatorName definition
ListPredefinedAttributesPaginatorName = Literal[
    "list_predefined_attributes",
]
```
## ListPromptsPaginatorName

```python
# ListPromptsPaginatorName usage example
from types_aiobotocore_connect.literals import ListPromptsPaginatorName

def get_value() -> ListPromptsPaginatorName:
    return "list_prompts"
```

```python
# ListPromptsPaginatorName definition
ListPromptsPaginatorName = Literal[
    "list_prompts",
]
```
## ListQueueQuickConnectsPaginatorName

```python
# ListQueueQuickConnectsPaginatorName usage example
from types_aiobotocore_connect.literals import ListQueueQuickConnectsPaginatorName

def get_value() -> ListQueueQuickConnectsPaginatorName:
    return "list_queue_quick_connects"
```

```python
# ListQueueQuickConnectsPaginatorName definition
ListQueueQuickConnectsPaginatorName = Literal[
    "list_queue_quick_connects",
]
```
## ListQueuesPaginatorName

```python
# ListQueuesPaginatorName usage example
from types_aiobotocore_connect.literals import ListQueuesPaginatorName

def get_value() -> ListQueuesPaginatorName:
    return "list_queues"
```

```python
# ListQueuesPaginatorName definition
ListQueuesPaginatorName = Literal[
    "list_queues",
]
```
## ListQuickConnectsPaginatorName

```python
# ListQuickConnectsPaginatorName usage example
from types_aiobotocore_connect.literals import ListQuickConnectsPaginatorName

def get_value() -> ListQuickConnectsPaginatorName:
    return "list_quick_connects"
```

```python
# ListQuickConnectsPaginatorName definition
ListQuickConnectsPaginatorName = Literal[
    "list_quick_connects",
]
```
## ListRoutingProfileManualAssignmentQueuesPaginatorName

```python
# ListRoutingProfileManualAssignmentQueuesPaginatorName usage example
from types_aiobotocore_connect.literals import ListRoutingProfileManualAssignmentQueuesPaginatorName

def get_value() -> ListRoutingProfileManualAssignmentQueuesPaginatorName:
    return "list_routing_profile_manual_assignment_queues"
```

```python
# ListRoutingProfileManualAssignmentQueuesPaginatorName definition
ListRoutingProfileManualAssignmentQueuesPaginatorName = Literal[
    "list_routing_profile_manual_assignment_queues",
]
```
## ListRoutingProfileQueuesPaginatorName

```python
# ListRoutingProfileQueuesPaginatorName usage example
from types_aiobotocore_connect.literals import ListRoutingProfileQueuesPaginatorName

def get_value() -> ListRoutingProfileQueuesPaginatorName:
    return "list_routing_profile_queues"
```

```python
# ListRoutingProfileQueuesPaginatorName definition
ListRoutingProfileQueuesPaginatorName = Literal[
    "list_routing_profile_queues",
]
```
## ListRoutingProfilesPaginatorName

```python
# ListRoutingProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import ListRoutingProfilesPaginatorName

def get_value() -> ListRoutingProfilesPaginatorName:
    return "list_routing_profiles"
```

```python
# ListRoutingProfilesPaginatorName definition
ListRoutingProfilesPaginatorName = Literal[
    "list_routing_profiles",
]
```
## ListRulesPaginatorName

```python
# ListRulesPaginatorName usage example
from types_aiobotocore_connect.literals import ListRulesPaginatorName

def get_value() -> ListRulesPaginatorName:
    return "list_rules"
```

```python
# ListRulesPaginatorName definition
ListRulesPaginatorName = Literal[
    "list_rules",
]
```
## ListSecurityKeysPaginatorName

```python
# ListSecurityKeysPaginatorName usage example
from types_aiobotocore_connect.literals import ListSecurityKeysPaginatorName

def get_value() -> ListSecurityKeysPaginatorName:
    return "list_security_keys"
```

```python
# ListSecurityKeysPaginatorName definition
ListSecurityKeysPaginatorName = Literal[
    "list_security_keys",
]
```
## ListSecurityProfileApplicationsPaginatorName

```python
# ListSecurityProfileApplicationsPaginatorName usage example
from types_aiobotocore_connect.literals import ListSecurityProfileApplicationsPaginatorName

def get_value() -> ListSecurityProfileApplicationsPaginatorName:
    return "list_security_profile_applications"
```

```python
# ListSecurityProfileApplicationsPaginatorName definition
ListSecurityProfileApplicationsPaginatorName = Literal[
    "list_security_profile_applications",
]
```
## ListSecurityProfileFlowModulesPaginatorName

```python
# ListSecurityProfileFlowModulesPaginatorName usage example
from types_aiobotocore_connect.literals import ListSecurityProfileFlowModulesPaginatorName

def get_value() -> ListSecurityProfileFlowModulesPaginatorName:
    return "list_security_profile_flow_modules"
```

```python
# ListSecurityProfileFlowModulesPaginatorName definition
ListSecurityProfileFlowModulesPaginatorName = Literal[
    "list_security_profile_flow_modules",
]
```
## ListSecurityProfilePermissionsPaginatorName

```python
# ListSecurityProfilePermissionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListSecurityProfilePermissionsPaginatorName

def get_value() -> ListSecurityProfilePermissionsPaginatorName:
    return "list_security_profile_permissions"
```

```python
# ListSecurityProfilePermissionsPaginatorName definition
ListSecurityProfilePermissionsPaginatorName = Literal[
    "list_security_profile_permissions",
]
```
## ListSecurityProfilesPaginatorName

```python
# ListSecurityProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import ListSecurityProfilesPaginatorName

def get_value() -> ListSecurityProfilesPaginatorName:
    return "list_security_profiles"
```

```python
# ListSecurityProfilesPaginatorName definition
ListSecurityProfilesPaginatorName = Literal[
    "list_security_profiles",
]
```
## ListTaskTemplatesPaginatorName

```python
# ListTaskTemplatesPaginatorName usage example
from types_aiobotocore_connect.literals import ListTaskTemplatesPaginatorName

def get_value() -> ListTaskTemplatesPaginatorName:
    return "list_task_templates"
```

```python
# ListTaskTemplatesPaginatorName definition
ListTaskTemplatesPaginatorName = Literal[
    "list_task_templates",
]
```
## ListTrafficDistributionGroupUsersPaginatorName

```python
# ListTrafficDistributionGroupUsersPaginatorName usage example
from types_aiobotocore_connect.literals import ListTrafficDistributionGroupUsersPaginatorName

def get_value() -> ListTrafficDistributionGroupUsersPaginatorName:
    return "list_traffic_distribution_group_users"
```

```python
# ListTrafficDistributionGroupUsersPaginatorName definition
ListTrafficDistributionGroupUsersPaginatorName = Literal[
    "list_traffic_distribution_group_users",
]
```
## ListTrafficDistributionGroupsPaginatorName

```python
# ListTrafficDistributionGroupsPaginatorName usage example
from types_aiobotocore_connect.literals import ListTrafficDistributionGroupsPaginatorName

def get_value() -> ListTrafficDistributionGroupsPaginatorName:
    return "list_traffic_distribution_groups"
```

```python
# ListTrafficDistributionGroupsPaginatorName definition
ListTrafficDistributionGroupsPaginatorName = Literal[
    "list_traffic_distribution_groups",
]
```
## ListUseCasesPaginatorName

```python
# ListUseCasesPaginatorName usage example
from types_aiobotocore_connect.literals import ListUseCasesPaginatorName

def get_value() -> ListUseCasesPaginatorName:
    return "list_use_cases"
```

```python
# ListUseCasesPaginatorName definition
ListUseCasesPaginatorName = Literal[
    "list_use_cases",
]
```
## ListUserHierarchyGroupsPaginatorName

```python
# ListUserHierarchyGroupsPaginatorName usage example
from types_aiobotocore_connect.literals import ListUserHierarchyGroupsPaginatorName

def get_value() -> ListUserHierarchyGroupsPaginatorName:
    return "list_user_hierarchy_groups"
```

```python
# ListUserHierarchyGroupsPaginatorName definition
ListUserHierarchyGroupsPaginatorName = Literal[
    "list_user_hierarchy_groups",
]
```
## ListUserProficienciesPaginatorName

```python
# ListUserProficienciesPaginatorName usage example
from types_aiobotocore_connect.literals import ListUserProficienciesPaginatorName

def get_value() -> ListUserProficienciesPaginatorName:
    return "list_user_proficiencies"
```

```python
# ListUserProficienciesPaginatorName definition
ListUserProficienciesPaginatorName = Literal[
    "list_user_proficiencies",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example
from types_aiobotocore_connect.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition
ListUsersPaginatorName = Literal[
    "list_users",
]
```
## ListViewVersionsPaginatorName

```python
# ListViewVersionsPaginatorName usage example
from types_aiobotocore_connect.literals import ListViewVersionsPaginatorName

def get_value() -> ListViewVersionsPaginatorName:
    return "list_view_versions"
```

```python
# ListViewVersionsPaginatorName definition
ListViewVersionsPaginatorName = Literal[
    "list_view_versions",
]
```
## ListViewsPaginatorName

```python
# ListViewsPaginatorName usage example
from types_aiobotocore_connect.literals import ListViewsPaginatorName

def get_value() -> ListViewsPaginatorName:
    return "list_views"
```

```python
# ListViewsPaginatorName definition
ListViewsPaginatorName = Literal[
    "list_views",
]
```
## ListWorkspacePagesPaginatorName

```python
# ListWorkspacePagesPaginatorName usage example
from types_aiobotocore_connect.literals import ListWorkspacePagesPaginatorName

def get_value() -> ListWorkspacePagesPaginatorName:
    return "list_workspace_pages"
```

```python
# ListWorkspacePagesPaginatorName definition
ListWorkspacePagesPaginatorName = Literal[
    "list_workspace_pages",
]
```
## ListWorkspacesPaginatorName

```python
# ListWorkspacesPaginatorName usage example
from types_aiobotocore_connect.literals import ListWorkspacesPaginatorName

def get_value() -> ListWorkspacesPaginatorName:
    return "list_workspaces"
```

```python
# ListWorkspacesPaginatorName definition
ListWorkspacesPaginatorName = Literal[
    "list_workspaces",
]
```
## MediaStreamTypeType

```python
# MediaStreamTypeType usage example
from types_aiobotocore_connect.literals import MediaStreamTypeType

def get_value() -> MediaStreamTypeType:
    return "AUDIO"
```

```python
# MediaStreamTypeType definition
MediaStreamTypeType = Literal[
    "AUDIO",
    "VIDEO",
]
```
## MediaTypeType

```python
# MediaTypeType usage example
from types_aiobotocore_connect.literals import MediaTypeType

def get_value() -> MediaTypeType:
    return "IMAGE_LOGO_DARK_FAVICON"
```

```python
# MediaTypeType definition
MediaTypeType = Literal[
    "IMAGE_LOGO_DARK_FAVICON",
    "IMAGE_LOGO_DARK_HORIZONTAL",
    "IMAGE_LOGO_LIGHT_FAVICON",
    "IMAGE_LOGO_LIGHT_HORIZONTAL",
]
```
## MeetingFeatureStatusType

```python
# MeetingFeatureStatusType usage example
from types_aiobotocore_connect.literals import MeetingFeatureStatusType

def get_value() -> MeetingFeatureStatusType:
    return "AVAILABLE"
```

```python
# MeetingFeatureStatusType definition
MeetingFeatureStatusType = Literal[
    "AVAILABLE",
    "UNAVAILABLE",
]
```
## MonitorCapabilityType

```python
# MonitorCapabilityType usage example
from types_aiobotocore_connect.literals import MonitorCapabilityType

def get_value() -> MonitorCapabilityType:
    return "BARGE"
```

```python
# MonitorCapabilityType definition
MonitorCapabilityType = Literal[
    "BARGE",
    "SILENT_MONITOR",
]
```
## MultiSelectQuestionRuleCategoryAutomationConditionType

```python
# MultiSelectQuestionRuleCategoryAutomationConditionType usage example
from types_aiobotocore_connect.literals import MultiSelectQuestionRuleCategoryAutomationConditionType

def get_value() -> MultiSelectQuestionRuleCategoryAutomationConditionType:
    return "NOT_PRESENT"
```

```python
# MultiSelectQuestionRuleCategoryAutomationConditionType definition
MultiSelectQuestionRuleCategoryAutomationConditionType = Literal[
    "NOT_PRESENT",
    "PRESENT",
]
```
## NextContactTypeType

```python
# NextContactTypeType usage example
from types_aiobotocore_connect.literals import NextContactTypeType

def get_value() -> NextContactTypeType:
    return "QUICK_CONNECT"
```

```python
# NextContactTypeType definition
NextContactTypeType = Literal[
    "QUICK_CONNECT",
]
```
## NotificationContentTypeType

```python
# NotificationContentTypeType usage example
from types_aiobotocore_connect.literals import NotificationContentTypeType

def get_value() -> NotificationContentTypeType:
    return "PLAIN_TEXT"
```

```python
# NotificationContentTypeType definition
NotificationContentTypeType = Literal[
    "PLAIN_TEXT",
]
```
## NotificationDeliveryTypeType

```python
# NotificationDeliveryTypeType usage example
from types_aiobotocore_connect.literals import NotificationDeliveryTypeType

def get_value() -> NotificationDeliveryTypeType:
    return "EMAIL"
```

```python
# NotificationDeliveryTypeType definition
NotificationDeliveryTypeType = Literal[
    "EMAIL",
]
```
## NumberComparisonTypeType

```python
# NumberComparisonTypeType usage example
from types_aiobotocore_connect.literals import NumberComparisonTypeType

def get_value() -> NumberComparisonTypeType:
    return "EQUAL"
```

```python
# NumberComparisonTypeType definition
NumberComparisonTypeType = Literal[
    "EQUAL",
    "GREATER",
    "GREATER_OR_EQUAL",
    "LESSER",
    "LESSER_OR_EQUAL",
    "NOT_EQUAL",
    "RANGE",
]
```
## NumericQuestionPropertyAutomationLabelType

```python
# NumericQuestionPropertyAutomationLabelType usage example
from types_aiobotocore_connect.literals import NumericQuestionPropertyAutomationLabelType

def get_value() -> NumericQuestionPropertyAutomationLabelType:
    return "AGENT_INTERACTION_AND_HOLD_DURATION"
```

```python
# NumericQuestionPropertyAutomationLabelType definition
NumericQuestionPropertyAutomationLabelType = Literal[
    "AGENT_INTERACTION_AND_HOLD_DURATION",
    "AGENT_INTERACTION_DURATION",
    "CONTACT_DURATION",
    "CUSTOMER_HOLD_TIME",
    "CUSTOMER_SENTIMENT_SCORE_WITH_AGENT",
    "CUSTOMER_SENTIMENT_SCORE_WITHOUT_AGENT",
    "LONGEST_HOLD_DURATION",
    "NON_TALK_TIME",
    "NON_TALK_TIME_PERCENTAGE",
    "NUMBER_OF_HOLDS",
    "NUMBER_OF_INTERRUPTIONS",
    "OVERALL_AGENT_SENTIMENT_SCORE",
    "OVERALL_CUSTOMER_SENTIMENT_SCORE",
]
```
## OperationalStatusType

```python
# OperationalStatusType usage example
from types_aiobotocore_connect.literals import OperationalStatusType

def get_value() -> OperationalStatusType:
    return "CLOSED"
```

```python
# OperationalStatusType definition
OperationalStatusType = Literal[
    "CLOSED",
    "OPEN",
]
```
## OutboundMessageSourceTypeType

```python
# OutboundMessageSourceTypeType usage example
from types_aiobotocore_connect.literals import OutboundMessageSourceTypeType

def get_value() -> OutboundMessageSourceTypeType:
    return "RAW"
```

```python
# OutboundMessageSourceTypeType definition
OutboundMessageSourceTypeType = Literal[
    "RAW",
    "TEMPLATE",
]
```
## OutboundStrategyTypeType

```python
# OutboundStrategyTypeType usage example
from types_aiobotocore_connect.literals import OutboundStrategyTypeType

def get_value() -> OutboundStrategyTypeType:
    return "AGENT_FIRST"
```

```python
# OutboundStrategyTypeType definition
OutboundStrategyTypeType = Literal[
    "AGENT_FIRST",
]
```
## OverrideDaysType

```python
# OverrideDaysType usage example
from types_aiobotocore_connect.literals import OverrideDaysType

def get_value() -> OverrideDaysType:
    return "FRIDAY"
```

```python
# OverrideDaysType definition
OverrideDaysType = Literal[
    "FRIDAY",
    "MONDAY",
    "SATURDAY",
    "SUNDAY",
    "THURSDAY",
    "TUESDAY",
    "WEDNESDAY",
]
```
## OverrideTypeType

```python
# OverrideTypeType usage example
from types_aiobotocore_connect.literals import OverrideTypeType

def get_value() -> OverrideTypeType:
    return "CLOSED"
```

```python
# OverrideTypeType definition
OverrideTypeType = Literal[
    "CLOSED",
    "OPEN",
    "STANDARD",
]
```
## ParticipantRoleType

```python
# ParticipantRoleType usage example
from types_aiobotocore_connect.literals import ParticipantRoleType

def get_value() -> ParticipantRoleType:
    return "AGENT"
```

```python
# ParticipantRoleType definition
ParticipantRoleType = Literal[
    "AGENT",
    "CUSTOM_BOT",
    "CUSTOMER",
    "SUPERVISOR",
    "SYSTEM",
]
```
## ParticipantStateType

```python
# ParticipantStateType usage example
from types_aiobotocore_connect.literals import ParticipantStateType

def get_value() -> ParticipantStateType:
    return "CONNECTED"
```

```python
# ParticipantStateType definition
ParticipantStateType = Literal[
    "CONNECTED",
    "DISCONNECTED",
    "INITIAL",
    "MISSED",
]
```
## ParticipantTimerActionType

```python
# ParticipantTimerActionType usage example
from types_aiobotocore_connect.literals import ParticipantTimerActionType

def get_value() -> ParticipantTimerActionType:
    return "Unset"
```

```python
# ParticipantTimerActionType definition
ParticipantTimerActionType = Literal[
    "Unset",
]
```
## ParticipantTimerTypeType

```python
# ParticipantTimerTypeType usage example
from types_aiobotocore_connect.literals import ParticipantTimerTypeType

def get_value() -> ParticipantTimerTypeType:
    return "DISCONNECT_NONCUSTOMER"
```

```python
# ParticipantTimerTypeType definition
ParticipantTimerTypeType = Literal[
    "DISCONNECT_NONCUSTOMER",
    "IDLE",
]
```
## ParticipantTypeType

```python
# ParticipantTypeType usage example
from types_aiobotocore_connect.literals import ParticipantTypeType

def get_value() -> ParticipantTypeType:
    return "AGENT"
```

```python
# ParticipantTypeType definition
ParticipantTypeType = Literal[
    "AGENT",
    "ALL",
    "CUSTOMER",
    "MANAGER",
    "THIRDPARTY",
]
```
## PhoneNumberCountryCodeType

```python
# PhoneNumberCountryCodeType usage example
from types_aiobotocore_connect.literals import PhoneNumberCountryCodeType

def get_value() -> PhoneNumberCountryCodeType:
    return "AD"
```

```python
# PhoneNumberCountryCodeType definition
PhoneNumberCountryCodeType = Literal[
    "AD",
    "AE",
    "AF",
    "AG",
    "AI",
    "AL",
    "AM",
    "AN",
    "AO",
    "AQ",
    "AR",
    "AS",
    "AT",
    "AU",
    "AW",
    "AZ",
    "BA",
    "BB",
    "BD",
    "BE",
    "BF",
    "BG",
    "BH",
    "BI",
    "BJ",
    "BL",
    "BM",
    "BN",
    "BO",
    "BR",
    "BS",
    "BT",
    "BW",
    "BY",
    "BZ",
    "CA",
    "CC",
    "CD",
    "CF",
    "CG",
    "CH",
    "CI",
    "CK",
    "CL",
    "CM",
    "CN",
    "CO",
    "CR",
    "CU",
    "CV",
    "CW",
    "CX",
    "CY",
    "CZ",
    "DE",
    "DJ",
    "DK",
    "DM",
    "DO",
    "DZ",
    "EC",
    "EE",
    "EG",
    "EH",
    "ER",
    "ES",
    "ET",
    "FI",
    "FJ",
    "FK",
    "FM",
    "FO",
    "FR",
    "GA",
    "GB",
    "GD",
    "GE",
    "GG",
    "GH",
    "GI",
    "GL",
    "GM",
    "GN",
    "GQ",
    "GR",
    "GT",
    "GU",
    "GW",
    "GY",
    "HK",
    "HN",
    "HR",
    "HT",
    "HU",
    "ID",
    "IE",
    "IL",
    "IM",
    "IN",
    "IO",
    "IQ",
    "IR",
    "IS",
    "IT",
    "JE",
    "JM",
    "JO",
    "JP",
    "KE",
    "KG",
    "KH",
    "KI",
    "KM",
    "KN",
    "KP",
    "KR",
    "KW",
    "KY",
    "KZ",
    "LA",
    "LB",
    "LC",
    "LI",
    "LK",
    "LR",
    "LS",
    "LT",
    "LU",
    "LV",
    "LY",
    "MA",
    "MC",
    "MD",
    "ME",
    "MF",
    "MG",
    "MH",
    "MK",
    "ML",
    "MM",
    "MN",
    "MO",
    "MP",
    "MR",
    "MS",
    "MT",
    "MU",
    "MV",
    "MW",
    "MX",
    "MY",
    "MZ",
    "NA",
    "NC",
    "NE",
    "NG",
    "NI",
    "NL",
    "NO",
    "NP",
    "NR",
    "NU",
    "NZ",
    "OM",
    "PA",
    "PE",
    "PF",
    "PG",
    "PH",
    "PK",
    "PL",
    "PM",
    "PN",
    "PR",
    "PT",
    "PW",
    "PY",
    "QA",
    "RE",
    "RO",
    "RS",
    "RU",
    "RW",
    "SA",
    "SB",
    "SC",
    "SD",
    "SE",
    "SG",
    "SH",
    "SI",
    "SJ",
    "SK",
    "SL",
    "SM",
    "SN",
    "SO",
    "SR",
    "ST",
    "SV",
    "SX",
    "SY",
    "SZ",
    "TC",
    "TD",
    "TG",
    "TH",
    "TJ",
    "TK",
    "TL",
    "TM",
    "TN",
    "TO",
    "TR",
    "TT",
    "TV",
    "TW",
    "TZ",
    "UA",
    "UG",
    "US",
    "UY",
    "UZ",
    "VA",
    "VC",
    "VE",
    "VG",
    "VI",
    "VN",
    "VU",
    "WF",
    "WS",
    "YE",
    "YT",
    "ZA",
    "ZM",
    "ZW",
]
```
## PhoneNumberTypeType

```python
# PhoneNumberTypeType usage example
from types_aiobotocore_connect.literals import PhoneNumberTypeType

def get_value() -> PhoneNumberTypeType:
    return "DID"
```

```python
# PhoneNumberTypeType definition
PhoneNumberTypeType = Literal[
    "DID",
    "SHARED",
    "SHORT_CODE",
    "THIRD_PARTY_DID",
    "THIRD_PARTY_TF",
    "TOLL_FREE",
    "UIFN",
]
```
## PhoneNumberWorkflowStatusType

```python
# PhoneNumberWorkflowStatusType usage example
from types_aiobotocore_connect.literals import PhoneNumberWorkflowStatusType

def get_value() -> PhoneNumberWorkflowStatusType:
    return "CLAIMED"
```

```python
# PhoneNumberWorkflowStatusType definition
PhoneNumberWorkflowStatusType = Literal[
    "CLAIMED",
    "FAILED",
    "IN_PROGRESS",
]
```
## PhoneTypeType

```python
# PhoneTypeType usage example
from types_aiobotocore_connect.literals import PhoneTypeType

def get_value() -> PhoneTypeType:
    return "DESK_PHONE"
```

```python
# PhoneTypeType definition
PhoneTypeType = Literal[
    "DESK_PHONE",
    "SOFT_PHONE",
]
```
## QuestionRuleCategoryAutomationConditionType

```python
# QuestionRuleCategoryAutomationConditionType usage example
from types_aiobotocore_connect.literals import QuestionRuleCategoryAutomationConditionType

def get_value() -> QuestionRuleCategoryAutomationConditionType:
    return "NOT_PRESENT"
```

```python
# QuestionRuleCategoryAutomationConditionType definition
QuestionRuleCategoryAutomationConditionType = Literal[
    "NOT_PRESENT",
    "PRESENT",
]
```
## QueueStatusType

```python
# QueueStatusType usage example
from types_aiobotocore_connect.literals import QueueStatusType

def get_value() -> QueueStatusType:
    return "DISABLED"
```

```python
# QueueStatusType definition
QueueStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## QueueTypeType

```python
# QueueTypeType usage example
from types_aiobotocore_connect.literals import QueueTypeType

def get_value() -> QueueTypeType:
    return "AGENT"
```

```python
# QueueTypeType definition
QueueTypeType = Literal[
    "AGENT",
    "STANDARD",
]
```
## QuickConnectTypeType

```python
# QuickConnectTypeType usage example
from types_aiobotocore_connect.literals import QuickConnectTypeType

def get_value() -> QuickConnectTypeType:
    return "FLOW"
```

```python
# QuickConnectTypeType definition
QuickConnectTypeType = Literal[
    "FLOW",
    "PHONE_NUMBER",
    "QUEUE",
    "USER",
]
```
## RealTimeContactAnalysisOutputTypeType

```python
# RealTimeContactAnalysisOutputTypeType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisOutputTypeType

def get_value() -> RealTimeContactAnalysisOutputTypeType:
    return "Raw"
```

```python
# RealTimeContactAnalysisOutputTypeType definition
RealTimeContactAnalysisOutputTypeType = Literal[
    "Raw",
    "Redacted",
]
```
## RealTimeContactAnalysisPostContactSummaryFailureCodeType

```python
# RealTimeContactAnalysisPostContactSummaryFailureCodeType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisPostContactSummaryFailureCodeType

def get_value() -> RealTimeContactAnalysisPostContactSummaryFailureCodeType:
    return "FAILED_SAFETY_GUIDELINES"
```

```python
# RealTimeContactAnalysisPostContactSummaryFailureCodeType definition
RealTimeContactAnalysisPostContactSummaryFailureCodeType = Literal[
    "FAILED_SAFETY_GUIDELINES",
    "INSUFFICIENT_CONVERSATION_CONTENT",
    "INTERNAL_ERROR",
    "INVALID_ANALYSIS_CONFIGURATION",
    "QUOTA_EXCEEDED",
]
```
## RealTimeContactAnalysisPostContactSummaryStatusType

```python
# RealTimeContactAnalysisPostContactSummaryStatusType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisPostContactSummaryStatusType

def get_value() -> RealTimeContactAnalysisPostContactSummaryStatusType:
    return "COMPLETED"
```

```python
# RealTimeContactAnalysisPostContactSummaryStatusType definition
RealTimeContactAnalysisPostContactSummaryStatusType = Literal[
    "COMPLETED",
    "FAILED",
]
```
## RealTimeContactAnalysisSegmentTypeType

```python
# RealTimeContactAnalysisSegmentTypeType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisSegmentTypeType

def get_value() -> RealTimeContactAnalysisSegmentTypeType:
    return "Attachments"
```

```python
# RealTimeContactAnalysisSegmentTypeType definition
RealTimeContactAnalysisSegmentTypeType = Literal[
    "Attachments",
    "Categories",
    "Event",
    "Issues",
    "PostContactSummary",
    "Transcript",
]
```
## RealTimeContactAnalysisSentimentLabelType

```python
# RealTimeContactAnalysisSentimentLabelType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisSentimentLabelType

def get_value() -> RealTimeContactAnalysisSentimentLabelType:
    return "NEGATIVE"
```

```python
# RealTimeContactAnalysisSentimentLabelType definition
RealTimeContactAnalysisSentimentLabelType = Literal[
    "NEGATIVE",
    "NEUTRAL",
    "POSITIVE",
]
```
## RealTimeContactAnalysisStatusType

```python
# RealTimeContactAnalysisStatusType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisStatusType

def get_value() -> RealTimeContactAnalysisStatusType:
    return "COMPLETED"
```

```python
# RealTimeContactAnalysisStatusType definition
RealTimeContactAnalysisStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## RealTimeContactAnalysisSupportedChannelType

```python
# RealTimeContactAnalysisSupportedChannelType usage example
from types_aiobotocore_connect.literals import RealTimeContactAnalysisSupportedChannelType

def get_value() -> RealTimeContactAnalysisSupportedChannelType:
    return "CHAT"
```

```python
# RealTimeContactAnalysisSupportedChannelType definition
RealTimeContactAnalysisSupportedChannelType = Literal[
    "CHAT",
    "VOICE",
]
```
## RecordingStatusType

```python
# RecordingStatusType usage example
from types_aiobotocore_connect.literals import RecordingStatusType

def get_value() -> RecordingStatusType:
    return "AVAILABLE"
```

```python
# RecordingStatusType definition
RecordingStatusType = Literal[
    "AVAILABLE",
    "DELETED",
]
```
## RecurrenceFrequencyType

```python
# RecurrenceFrequencyType usage example
from types_aiobotocore_connect.literals import RecurrenceFrequencyType

def get_value() -> RecurrenceFrequencyType:
    return "MONTHLY"
```

```python
# RecurrenceFrequencyType definition
RecurrenceFrequencyType = Literal[
    "MONTHLY",
    "WEEKLY",
    "YEARLY",
]
```
## ReferenceStatusType

```python
# ReferenceStatusType usage example
from types_aiobotocore_connect.literals import ReferenceStatusType

def get_value() -> ReferenceStatusType:
    return "APPROVED"
```

```python
# ReferenceStatusType definition
ReferenceStatusType = Literal[
    "APPROVED",
    "AVAILABLE",
    "DELETED",
    "FAILED",
    "PROCESSING",
    "REJECTED",
]
```
## ReferenceTypeType

```python
# ReferenceTypeType usage example
from types_aiobotocore_connect.literals import ReferenceTypeType

def get_value() -> ReferenceTypeType:
    return "ATTACHMENT"
```

```python
# ReferenceTypeType definition
ReferenceTypeType = Literal[
    "ATTACHMENT",
    "CONTACT_ANALYSIS",
    "DATE",
    "EMAIL",
    "EMAIL_MESSAGE",
    "EMAIL_MESSAGE_PLAIN_TEXT",
    "NUMBER",
    "STRING",
    "URL",
]
```
## RehydrationTypeType

```python
# RehydrationTypeType usage example
from types_aiobotocore_connect.literals import RehydrationTypeType

def get_value() -> RehydrationTypeType:
    return "ENTIRE_PAST_SESSION"
```

```python
# RehydrationTypeType definition
RehydrationTypeType = Literal[
    "ENTIRE_PAST_SESSION",
    "FROM_SEGMENT",
]
```
## ResponseModeType

```python
# ResponseModeType usage example
from types_aiobotocore_connect.literals import ResponseModeType

def get_value() -> ResponseModeType:
    return "COMPLETE"
```

```python
# ResponseModeType definition
ResponseModeType = Literal[
    "COMPLETE",
    "INCREMENTAL",
]
```
## RoutingCriteriaStepStatusType

```python
# RoutingCriteriaStepStatusType usage example
from types_aiobotocore_connect.literals import RoutingCriteriaStepStatusType

def get_value() -> RoutingCriteriaStepStatusType:
    return "ACTIVE"
```

```python
# RoutingCriteriaStepStatusType definition
RoutingCriteriaStepStatusType = Literal[
    "ACTIVE",
    "EXPIRED",
    "INACTIVE",
    "JOINED",
]
```
## RulePublishStatusType

```python
# RulePublishStatusType usage example
from types_aiobotocore_connect.literals import RulePublishStatusType

def get_value() -> RulePublishStatusType:
    return "DRAFT"
```

```python
# RulePublishStatusType definition
RulePublishStatusType = Literal[
    "DRAFT",
    "PUBLISHED",
]
```
## ScreenShareCapabilityType

```python
# ScreenShareCapabilityType usage example
from types_aiobotocore_connect.literals import ScreenShareCapabilityType

def get_value() -> ScreenShareCapabilityType:
    return "SEND"
```

```python
# ScreenShareCapabilityType definition
ScreenShareCapabilityType = Literal[
    "SEND",
]
```
## SearchAgentStatusesPaginatorName

```python
# SearchAgentStatusesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchAgentStatusesPaginatorName

def get_value() -> SearchAgentStatusesPaginatorName:
    return "search_agent_statuses"
```

```python
# SearchAgentStatusesPaginatorName definition
SearchAgentStatusesPaginatorName = Literal[
    "search_agent_statuses",
]
```
## SearchAvailablePhoneNumbersPaginatorName

```python
# SearchAvailablePhoneNumbersPaginatorName usage example
from types_aiobotocore_connect.literals import SearchAvailablePhoneNumbersPaginatorName

def get_value() -> SearchAvailablePhoneNumbersPaginatorName:
    return "search_available_phone_numbers"
```

```python
# SearchAvailablePhoneNumbersPaginatorName definition
SearchAvailablePhoneNumbersPaginatorName = Literal[
    "search_available_phone_numbers",
]
```
## SearchContactFlowModulesPaginatorName

```python
# SearchContactFlowModulesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchContactFlowModulesPaginatorName

def get_value() -> SearchContactFlowModulesPaginatorName:
    return "search_contact_flow_modules"
```

```python
# SearchContactFlowModulesPaginatorName definition
SearchContactFlowModulesPaginatorName = Literal[
    "search_contact_flow_modules",
]
```
## SearchContactFlowsPaginatorName

```python
# SearchContactFlowsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchContactFlowsPaginatorName

def get_value() -> SearchContactFlowsPaginatorName:
    return "search_contact_flows"
```

```python
# SearchContactFlowsPaginatorName definition
SearchContactFlowsPaginatorName = Literal[
    "search_contact_flows",
]
```
## SearchContactsMatchTypeType

```python
# SearchContactsMatchTypeType usage example
from types_aiobotocore_connect.literals import SearchContactsMatchTypeType

def get_value() -> SearchContactsMatchTypeType:
    return "MATCH_ALL"
```

```python
# SearchContactsMatchTypeType definition
SearchContactsMatchTypeType = Literal[
    "MATCH_ALL",
    "MATCH_ANY",
    "MATCH_EXACT",
    "MATCH_NONE",
]
```
## SearchContactsPaginatorName

```python
# SearchContactsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchContactsPaginatorName

def get_value() -> SearchContactsPaginatorName:
    return "search_contacts"
```

```python
# SearchContactsPaginatorName definition
SearchContactsPaginatorName = Literal[
    "search_contacts",
]
```
## SearchContactsTimeRangeConditionTypeType

```python
# SearchContactsTimeRangeConditionTypeType usage example
from types_aiobotocore_connect.literals import SearchContactsTimeRangeConditionTypeType

def get_value() -> SearchContactsTimeRangeConditionTypeType:
    return "NOT_EXISTS"
```

```python
# SearchContactsTimeRangeConditionTypeType definition
SearchContactsTimeRangeConditionTypeType = Literal[
    "NOT_EXISTS",
]
```
## SearchContactsTimeRangeTypeType

```python
# SearchContactsTimeRangeTypeType usage example
from types_aiobotocore_connect.literals import SearchContactsTimeRangeTypeType

def get_value() -> SearchContactsTimeRangeTypeType:
    return "CONNECTED_TO_AGENT_TIMESTAMP"
```

```python
# SearchContactsTimeRangeTypeType definition
SearchContactsTimeRangeTypeType = Literal[
    "CONNECTED_TO_AGENT_TIMESTAMP",
    "DISCONNECT_TIMESTAMP",
    "ENQUEUE_TIMESTAMP",
    "INITIATION_TIMESTAMP",
    "SCHEDULED_TIMESTAMP",
]
```
## SearchDataTablesPaginatorName

```python
# SearchDataTablesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchDataTablesPaginatorName

def get_value() -> SearchDataTablesPaginatorName:
    return "search_data_tables"
```

```python
# SearchDataTablesPaginatorName definition
SearchDataTablesPaginatorName = Literal[
    "search_data_tables",
]
```
## SearchHoursOfOperationOverridesPaginatorName

```python
# SearchHoursOfOperationOverridesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchHoursOfOperationOverridesPaginatorName

def get_value() -> SearchHoursOfOperationOverridesPaginatorName:
    return "search_hours_of_operation_overrides"
```

```python
# SearchHoursOfOperationOverridesPaginatorName definition
SearchHoursOfOperationOverridesPaginatorName = Literal[
    "search_hours_of_operation_overrides",
]
```
## SearchHoursOfOperationsPaginatorName

```python
# SearchHoursOfOperationsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchHoursOfOperationsPaginatorName

def get_value() -> SearchHoursOfOperationsPaginatorName:
    return "search_hours_of_operations"
```

```python
# SearchHoursOfOperationsPaginatorName definition
SearchHoursOfOperationsPaginatorName = Literal[
    "search_hours_of_operations",
]
```
## SearchPredefinedAttributesPaginatorName

```python
# SearchPredefinedAttributesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchPredefinedAttributesPaginatorName

def get_value() -> SearchPredefinedAttributesPaginatorName:
    return "search_predefined_attributes"
```

```python
# SearchPredefinedAttributesPaginatorName definition
SearchPredefinedAttributesPaginatorName = Literal[
    "search_predefined_attributes",
]
```
## SearchPromptsPaginatorName

```python
# SearchPromptsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchPromptsPaginatorName

def get_value() -> SearchPromptsPaginatorName:
    return "search_prompts"
```

```python
# SearchPromptsPaginatorName definition
SearchPromptsPaginatorName = Literal[
    "search_prompts",
]
```
## SearchQueuesPaginatorName

```python
# SearchQueuesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchQueuesPaginatorName

def get_value() -> SearchQueuesPaginatorName:
    return "search_queues"
```

```python
# SearchQueuesPaginatorName definition
SearchQueuesPaginatorName = Literal[
    "search_queues",
]
```
## SearchQuickConnectsPaginatorName

```python
# SearchQuickConnectsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchQuickConnectsPaginatorName

def get_value() -> SearchQuickConnectsPaginatorName:
    return "search_quick_connects"
```

```python
# SearchQuickConnectsPaginatorName definition
SearchQuickConnectsPaginatorName = Literal[
    "search_quick_connects",
]
```
## SearchResourceTagsPaginatorName

```python
# SearchResourceTagsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchResourceTagsPaginatorName

def get_value() -> SearchResourceTagsPaginatorName:
    return "search_resource_tags"
```

```python
# SearchResourceTagsPaginatorName definition
SearchResourceTagsPaginatorName = Literal[
    "search_resource_tags",
]
```
## SearchRoutingProfilesPaginatorName

```python
# SearchRoutingProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchRoutingProfilesPaginatorName

def get_value() -> SearchRoutingProfilesPaginatorName:
    return "search_routing_profiles"
```

```python
# SearchRoutingProfilesPaginatorName definition
SearchRoutingProfilesPaginatorName = Literal[
    "search_routing_profiles",
]
```
## SearchSecurityProfilesPaginatorName

```python
# SearchSecurityProfilesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchSecurityProfilesPaginatorName

def get_value() -> SearchSecurityProfilesPaginatorName:
    return "search_security_profiles"
```

```python
# SearchSecurityProfilesPaginatorName definition
SearchSecurityProfilesPaginatorName = Literal[
    "search_security_profiles",
]
```
## SearchUserHierarchyGroupsPaginatorName

```python
# SearchUserHierarchyGroupsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchUserHierarchyGroupsPaginatorName

def get_value() -> SearchUserHierarchyGroupsPaginatorName:
    return "search_user_hierarchy_groups"
```

```python
# SearchUserHierarchyGroupsPaginatorName definition
SearchUserHierarchyGroupsPaginatorName = Literal[
    "search_user_hierarchy_groups",
]
```
## SearchUsersPaginatorName

```python
# SearchUsersPaginatorName usage example
from types_aiobotocore_connect.literals import SearchUsersPaginatorName

def get_value() -> SearchUsersPaginatorName:
    return "search_users"
```

```python
# SearchUsersPaginatorName definition
SearchUsersPaginatorName = Literal[
    "search_users",
]
```
## SearchViewsPaginatorName

```python
# SearchViewsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchViewsPaginatorName

def get_value() -> SearchViewsPaginatorName:
    return "search_views"
```

```python
# SearchViewsPaginatorName definition
SearchViewsPaginatorName = Literal[
    "search_views",
]
```
## SearchVocabulariesPaginatorName

```python
# SearchVocabulariesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchVocabulariesPaginatorName

def get_value() -> SearchVocabulariesPaginatorName:
    return "search_vocabularies"
```

```python
# SearchVocabulariesPaginatorName definition
SearchVocabulariesPaginatorName = Literal[
    "search_vocabularies",
]
```
## SearchWorkspaceAssociationsPaginatorName

```python
# SearchWorkspaceAssociationsPaginatorName usage example
from types_aiobotocore_connect.literals import SearchWorkspaceAssociationsPaginatorName

def get_value() -> SearchWorkspaceAssociationsPaginatorName:
    return "search_workspace_associations"
```

```python
# SearchWorkspaceAssociationsPaginatorName definition
SearchWorkspaceAssociationsPaginatorName = Literal[
    "search_workspace_associations",
]
```
## SearchWorkspacesPaginatorName

```python
# SearchWorkspacesPaginatorName usage example
from types_aiobotocore_connect.literals import SearchWorkspacesPaginatorName

def get_value() -> SearchWorkspacesPaginatorName:
    return "search_workspaces"
```

```python
# SearchWorkspacesPaginatorName definition
SearchWorkspacesPaginatorName = Literal[
    "search_workspaces",
]
```
## SearchableQueueTypeType

```python
# SearchableQueueTypeType usage example
from types_aiobotocore_connect.literals import SearchableQueueTypeType

def get_value() -> SearchableQueueTypeType:
    return "STANDARD"
```

```python
# SearchableQueueTypeType definition
SearchableQueueTypeType = Literal[
    "STANDARD",
]
```
## SingleSelectQuestionRuleCategoryAutomationConditionType

```python
# SingleSelectQuestionRuleCategoryAutomationConditionType usage example
from types_aiobotocore_connect.literals import SingleSelectQuestionRuleCategoryAutomationConditionType

def get_value() -> SingleSelectQuestionRuleCategoryAutomationConditionType:
    return "NOT_PRESENT"
```

```python
# SingleSelectQuestionRuleCategoryAutomationConditionType definition
SingleSelectQuestionRuleCategoryAutomationConditionType = Literal[
    "NOT_PRESENT",
    "PRESENT",
]
```
## SlaAssignmentTypeType

```python
# SlaAssignmentTypeType usage example
from types_aiobotocore_connect.literals import SlaAssignmentTypeType

def get_value() -> SlaAssignmentTypeType:
    return "CASES"
```

```python
# SlaAssignmentTypeType definition
SlaAssignmentTypeType = Literal[
    "CASES",
]
```
## SlaTypeType

```python
# SlaTypeType usage example
from types_aiobotocore_connect.literals import SlaTypeType

def get_value() -> SlaTypeType:
    return "CaseField"
```

```python
# SlaTypeType definition
SlaTypeType = Literal[
    "CaseField",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_connect.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASCENDING"
```

```python
# SortOrderType definition
SortOrderType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## SortableFieldNameType

```python
# SortableFieldNameType usage example
from types_aiobotocore_connect.literals import SortableFieldNameType

def get_value() -> SortableFieldNameType:
    return "CHANNEL"
```

```python
# SortableFieldNameType definition
SortableFieldNameType = Literal[
    "CHANNEL",
    "CONNECTED_TO_AGENT_TIMESTAMP",
    "DISCONNECT_TIMESTAMP",
    "EXPIRY_TIMESTAMP",
    "INITIATION_METHOD",
    "INITIATION_TIMESTAMP",
    "SCHEDULED_TIMESTAMP",
]
```
## SourceTypeType

```python
# SourceTypeType usage example
from types_aiobotocore_connect.literals import SourceTypeType

def get_value() -> SourceTypeType:
    return "CASES"
```

```python
# SourceTypeType definition
SourceTypeType = Literal[
    "CASES",
    "SALESFORCE",
    "ZENDESK",
]
```
## StatisticType

```python
# StatisticType usage example
from types_aiobotocore_connect.literals import StatisticType

def get_value() -> StatisticType:
    return "AVG"
```

```python
# StatisticType definition
StatisticType = Literal[
    "AVG",
    "MAX",
    "SUM",
]
```
## StatusType

```python
# StatusType usage example
from types_aiobotocore_connect.literals import StatusType

def get_value() -> StatusType:
    return "COMPLETE"
```

```python
# StatusType definition
StatusType = Literal[
    "COMPLETE",
    "DELETED",
    "IN_PROGRESS",
]
```
## StorageTypeType

```python
# StorageTypeType usage example
from types_aiobotocore_connect.literals import StorageTypeType

def get_value() -> StorageTypeType:
    return "KINESIS_FIREHOSE"
```

```python
# StorageTypeType definition
StorageTypeType = Literal[
    "KINESIS_FIREHOSE",
    "KINESIS_STREAM",
    "KINESIS_VIDEO_STREAM",
    "S3",
]
```
## StringComparisonTypeType

```python
# StringComparisonTypeType usage example
from types_aiobotocore_connect.literals import StringComparisonTypeType

def get_value() -> StringComparisonTypeType:
    return "CONTAINS"
```

```python
# StringComparisonTypeType definition
StringComparisonTypeType = Literal[
    "CONTAINS",
    "EXACT",
    "STARTS_WITH",
]
```
## TargetListTypeType

```python
# TargetListTypeType usage example
from types_aiobotocore_connect.literals import TargetListTypeType

def get_value() -> TargetListTypeType:
    return "PROFICIENCIES"
```

```python
# TargetListTypeType definition
TargetListTypeType = Literal[
    "PROFICIENCIES",
]
```
## TaskTemplateFieldTypeType

```python
# TaskTemplateFieldTypeType usage example
from types_aiobotocore_connect.literals import TaskTemplateFieldTypeType

def get_value() -> TaskTemplateFieldTypeType:
    return "BOOLEAN"
```

```python
# TaskTemplateFieldTypeType definition
TaskTemplateFieldTypeType = Literal[
    "BOOLEAN",
    "DATE_TIME",
    "DESCRIPTION",
    "EMAIL",
    "EXPIRY_DURATION",
    "NAME",
    "NUMBER",
    "QUICK_CONNECT",
    "SCHEDULED_TIME",
    "SELF_ASSIGN",
    "SINGLE_SELECT",
    "TEXT",
    "TEXT_AREA",
    "URL",
]
```
## TaskTemplateStatusType

```python
# TaskTemplateStatusType usage example
from types_aiobotocore_connect.literals import TaskTemplateStatusType

def get_value() -> TaskTemplateStatusType:
    return "ACTIVE"
```

```python
# TaskTemplateStatusType definition
TaskTemplateStatusType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## TimerEligibleParticipantRolesType

```python
# TimerEligibleParticipantRolesType usage example
from types_aiobotocore_connect.literals import TimerEligibleParticipantRolesType

def get_value() -> TimerEligibleParticipantRolesType:
    return "AGENT"
```

```python
# TimerEligibleParticipantRolesType definition
TimerEligibleParticipantRolesType = Literal[
    "AGENT",
    "CUSTOMER",
]
```
## TrafficDistributionGroupStatusType

```python
# TrafficDistributionGroupStatusType usage example
from types_aiobotocore_connect.literals import TrafficDistributionGroupStatusType

def get_value() -> TrafficDistributionGroupStatusType:
    return "ACTIVE"
```

```python
# TrafficDistributionGroupStatusType definition
TrafficDistributionGroupStatusType = Literal[
    "ACTIVE",
    "CREATION_FAILED",
    "CREATION_IN_PROGRESS",
    "DELETION_FAILED",
    "PENDING_DELETION",
    "UPDATE_IN_PROGRESS",
]
```
## TrafficTypeType

```python
# TrafficTypeType usage example
from types_aiobotocore_connect.literals import TrafficTypeType

def get_value() -> TrafficTypeType:
    return "CAMPAIGN"
```

```python
# TrafficTypeType definition
TrafficTypeType = Literal[
    "CAMPAIGN",
    "GENERAL",
]
```
## UnitType

```python
# UnitType usage example
from types_aiobotocore_connect.literals import UnitType

def get_value() -> UnitType:
    return "COUNT"
```

```python
# UnitType definition
UnitType = Literal[
    "COUNT",
    "PERCENT",
    "SECONDS",
]
```
## UseCaseTypeType

```python
# UseCaseTypeType usage example
from types_aiobotocore_connect.literals import UseCaseTypeType

def get_value() -> UseCaseTypeType:
    return "CONNECT_CAMPAIGNS"
```

```python
# UseCaseTypeType definition
UseCaseTypeType = Literal[
    "CONNECT_CAMPAIGNS",
    "RULES_EVALUATION",
]
```
## VideoCapabilityType

```python
# VideoCapabilityType usage example
from types_aiobotocore_connect.literals import VideoCapabilityType

def get_value() -> VideoCapabilityType:
    return "SEND"
```

```python
# VideoCapabilityType definition
VideoCapabilityType = Literal[
    "SEND",
]
```
## ViewStatusType

```python
# ViewStatusType usage example
from types_aiobotocore_connect.literals import ViewStatusType

def get_value() -> ViewStatusType:
    return "PUBLISHED"
```

```python
# ViewStatusType definition
ViewStatusType = Literal[
    "PUBLISHED",
    "SAVED",
]
```
## ViewTypeType

```python
# ViewTypeType usage example
from types_aiobotocore_connect.literals import ViewTypeType

def get_value() -> ViewTypeType:
    return "AWS_MANAGED"
```

```python
# ViewTypeType definition
ViewTypeType = Literal[
    "AWS_MANAGED",
    "CUSTOMER_MANAGED",
]
```
## VisibilityType

```python
# VisibilityType usage example
from types_aiobotocore_connect.literals import VisibilityType

def get_value() -> VisibilityType:
    return "ALL"
```

```python
# VisibilityType definition
VisibilityType = Literal[
    "ALL",
    "ASSIGNED",
    "NONE",
]
```
## VocabularyLanguageCodeType

```python
# VocabularyLanguageCodeType usage example
from types_aiobotocore_connect.literals import VocabularyLanguageCodeType

def get_value() -> VocabularyLanguageCodeType:
    return "ar-AE"
```

```python
# VocabularyLanguageCodeType definition
VocabularyLanguageCodeType = Literal[
    "ar-AE",
    "ca-ES",
    "da-DK",
    "de-CH",
    "de-DE",
    "en-AB",
    "en-AU",
    "en-GB",
    "en-IE",
    "en-IN",
    "en-NZ",
    "en-US",
    "en-WL",
    "en-ZA",
    "es-ES",
    "es-US",
    "fi-FI",
    "fr-CA",
    "fr-FR",
    "hi-IN",
    "id-ID",
    "it-IT",
    "ja-JP",
    "ko-KR",
    "ms-MY",
    "nl-NL",
    "no-NO",
    "pl-PL",
    "pt-BR",
    "pt-PT",
    "sv-SE",
    "tl-PH",
    "zh-CN",
]
```
## VocabularyStateType

```python
# VocabularyStateType usage example
from types_aiobotocore_connect.literals import VocabularyStateType

def get_value() -> VocabularyStateType:
    return "ACTIVE"
```

```python
# VocabularyStateType definition
VocabularyStateType = Literal[
    "ACTIVE",
    "CREATION_FAILED",
    "CREATION_IN_PROGRESS",
    "DELETE_IN_PROGRESS",
]
```
## VoiceRecordingTrackType

```python
# VoiceRecordingTrackType usage example
from types_aiobotocore_connect.literals import VoiceRecordingTrackType

def get_value() -> VoiceRecordingTrackType:
    return "ALL"
```

```python
# VoiceRecordingTrackType definition
VoiceRecordingTrackType = Literal[
    "ALL",
    "FROM_AGENT",
    "TO_AGENT",
]
```
## WorkspaceFontFamilyType

```python
# WorkspaceFontFamilyType usage example
from types_aiobotocore_connect.literals import WorkspaceFontFamilyType

def get_value() -> WorkspaceFontFamilyType:
    return "Arial"
```

```python
# WorkspaceFontFamilyType definition
WorkspaceFontFamilyType = Literal[
    "Arial",
    "Courier New",
    "Georgia",
    "Times New Roman",
    "Trebuchet",
    "Verdana",
]
```
## ConnectServiceName

```python
# ConnectServiceName usage example
from types_aiobotocore_connect.literals import ConnectServiceName

def get_value() -> ConnectServiceName:
    return "connect"
```

```python
# ConnectServiceName definition
ConnectServiceName = Literal[
    "connect",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_connect.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition
ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "aiops",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-region-switch",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupsearch",
    "batch",
    "bcm-dashboards",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bcm-recommended-actions",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-agentcore",
    "bedrock-agentcore-control",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "compute-optimizer-automation",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "ds-data",
    "dsql",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "eks-auth",
    "elasticache",
    "elasticbeanstalk",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "evs",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "gameliftstreams",
    "geo-maps",
    "geo-places",
    "geo-routes",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-managed-integrations",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "keyspacesstreams",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "launch-wizard",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mpa",
    "mq",
    "mturk",
    "mwaa",
    "mwaa-serverless",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "nova-act",
    "oam",
    "observabilityadmin",
    "odb",
    "omics",
    "opensearch",
    "opensearchserverless",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-account",
    "partnercentral-benefits",
    "partnercentral-channel",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53globalresolver",
    "route53profiles",
    "route53resolver",
    "rtbfabric",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "s3vectors",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "security-ir",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "signin",
    "simspaceweaver",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-guiconnect",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wickr",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-instances",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_connect.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition
ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_connect.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_metric_data"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "get_metric_data",
    "list_agent_statuses",
    "list_approved_origins",
    "list_authentication_profiles",
    "list_bots",
    "list_child_hours_of_operations",
    "list_contact_evaluations",
    "list_contact_flow_module_aliases",
    "list_contact_flow_module_versions",
    "list_contact_flow_modules",
    "list_contact_flow_versions",
    "list_contact_flows",
    "list_contact_references",
    "list_data_table_attributes",
    "list_data_table_primary_values",
    "list_data_table_values",
    "list_data_tables",
    "list_default_vocabularies",
    "list_entity_security_profiles",
    "list_evaluation_form_versions",
    "list_evaluation_forms",
    "list_flow_associations",
    "list_hours_of_operation_overrides",
    "list_hours_of_operations",
    "list_instance_attributes",
    "list_instance_storage_configs",
    "list_instances",
    "list_integration_associations",
    "list_lambda_functions",
    "list_lex_bots",
    "list_phone_numbers",
    "list_phone_numbers_v2",
    "list_predefined_attributes",
    "list_prompts",
    "list_queue_quick_connects",
    "list_queues",
    "list_quick_connects",
    "list_routing_profile_manual_assignment_queues",
    "list_routing_profile_queues",
    "list_routing_profiles",
    "list_rules",
    "list_security_keys",
    "list_security_profile_applications",
    "list_security_profile_flow_modules",
    "list_security_profile_permissions",
    "list_security_profiles",
    "list_task_templates",
    "list_traffic_distribution_group_users",
    "list_traffic_distribution_groups",
    "list_use_cases",
    "list_user_hierarchy_groups",
    "list_user_proficiencies",
    "list_users",
    "list_view_versions",
    "list_views",
    "list_workspace_pages",
    "list_workspaces",
    "search_agent_statuses",
    "search_available_phone_numbers",
    "search_contact_flow_modules",
    "search_contact_flows",
    "search_contacts",
    "search_data_tables",
    "search_hours_of_operation_overrides",
    "search_hours_of_operations",
    "search_predefined_attributes",
    "search_prompts",
    "search_queues",
    "search_quick_connects",
    "search_resource_tags",
    "search_routing_profiles",
    "search_security_profiles",
    "search_user_hierarchy_groups",
    "search_users",
    "search_views",
    "search_vocabularies",
    "search_workspace_associations",
    "search_workspaces",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_connect.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition
RegionName = Literal[
    "af-south-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-2",
    "us-east-1",
    "us-west-2",
]
```
