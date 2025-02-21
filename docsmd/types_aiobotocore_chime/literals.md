# Literals

> [Index](../README.md) > [Chime](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## AccountStatusType

```python
# AccountStatusType usage example
from types_aiobotocore_chime.literals import AccountStatusType

def get_value() -> AccountStatusType:
    return "Active"
```

```python
# AccountStatusType definition
AccountStatusType = Literal[
    "Active",
    "Suspended",
]
```
## AccountTypeType

```python
# AccountTypeType usage example
from types_aiobotocore_chime.literals import AccountTypeType

def get_value() -> AccountTypeType:
    return "EnterpriseDirectory"
```

```python
# AccountTypeType definition
AccountTypeType = Literal[
    "EnterpriseDirectory",
    "EnterpriseLWA",
    "EnterpriseOIDC",
    "Team",
]
```
## AppInstanceDataTypeType

```python
# AppInstanceDataTypeType usage example
from types_aiobotocore_chime.literals import AppInstanceDataTypeType

def get_value() -> AppInstanceDataTypeType:
    return "Channel"
```

```python
# AppInstanceDataTypeType definition
AppInstanceDataTypeType = Literal[
    "Channel",
    "ChannelMessage",
]
```
## ArtifactsStateType

```python
# ArtifactsStateType usage example
from types_aiobotocore_chime.literals import ArtifactsStateType

def get_value() -> ArtifactsStateType:
    return "Disabled"
```

```python
# ArtifactsStateType definition
ArtifactsStateType = Literal[
    "Disabled",
    "Enabled",
]
```
## AudioMuxTypeType

```python
# AudioMuxTypeType usage example
from types_aiobotocore_chime.literals import AudioMuxTypeType

def get_value() -> AudioMuxTypeType:
    return "AudioOnly"
```

```python
# AudioMuxTypeType definition
AudioMuxTypeType = Literal[
    "AudioOnly",
    "AudioWithActiveSpeakerVideo",
]
```
## BotTypeType

```python
# BotTypeType usage example
from types_aiobotocore_chime.literals import BotTypeType

def get_value() -> BotTypeType:
    return "ChatBot"
```

```python
# BotTypeType definition
BotTypeType = Literal[
    "ChatBot",
]
```
## CallingNameStatusType

```python
# CallingNameStatusType usage example
from types_aiobotocore_chime.literals import CallingNameStatusType

def get_value() -> CallingNameStatusType:
    return "Unassigned"
```

```python
# CallingNameStatusType definition
CallingNameStatusType = Literal[
    "Unassigned",
    "UpdateFailed",
    "UpdateInProgress",
    "UpdateSucceeded",
]
```
## CapabilityType

```python
# CapabilityType usage example
from types_aiobotocore_chime.literals import CapabilityType

def get_value() -> CapabilityType:
    return "SMS"
```

```python
# CapabilityType definition
CapabilityType = Literal[
    "SMS",
    "Voice",
]
```
## ChannelMembershipTypeType

```python
# ChannelMembershipTypeType usage example
from types_aiobotocore_chime.literals import ChannelMembershipTypeType

def get_value() -> ChannelMembershipTypeType:
    return "DEFAULT"
```

```python
# ChannelMembershipTypeType definition
ChannelMembershipTypeType = Literal[
    "DEFAULT",
    "HIDDEN",
]
```
## ChannelMessagePersistenceTypeType

```python
# ChannelMessagePersistenceTypeType usage example
from types_aiobotocore_chime.literals import ChannelMessagePersistenceTypeType

def get_value() -> ChannelMessagePersistenceTypeType:
    return "NON_PERSISTENT"
```

```python
# ChannelMessagePersistenceTypeType definition
ChannelMessagePersistenceTypeType = Literal[
    "NON_PERSISTENT",
    "PERSISTENT",
]
```
## ChannelMessageTypeType

```python
# ChannelMessageTypeType usage example
from types_aiobotocore_chime.literals import ChannelMessageTypeType

def get_value() -> ChannelMessageTypeType:
    return "CONTROL"
```

```python
# ChannelMessageTypeType definition
ChannelMessageTypeType = Literal[
    "CONTROL",
    "STANDARD",
]
```
## ChannelModeType

```python
# ChannelModeType usage example
from types_aiobotocore_chime.literals import ChannelModeType

def get_value() -> ChannelModeType:
    return "RESTRICTED"
```

```python
# ChannelModeType definition
ChannelModeType = Literal[
    "RESTRICTED",
    "UNRESTRICTED",
]
```
## ChannelPrivacyType

```python
# ChannelPrivacyType usage example
from types_aiobotocore_chime.literals import ChannelPrivacyType

def get_value() -> ChannelPrivacyType:
    return "PRIVATE"
```

```python
# ChannelPrivacyType definition
ChannelPrivacyType = Literal[
    "PRIVATE",
    "PUBLIC",
]
```
## ContentMuxTypeType

```python
# ContentMuxTypeType usage example
from types_aiobotocore_chime.literals import ContentMuxTypeType

def get_value() -> ContentMuxTypeType:
    return "ContentOnly"
```

```python
# ContentMuxTypeType definition
ContentMuxTypeType = Literal[
    "ContentOnly",
]
```
## EmailStatusType

```python
# EmailStatusType usage example
from types_aiobotocore_chime.literals import EmailStatusType

def get_value() -> EmailStatusType:
    return "Failed"
```

```python
# EmailStatusType definition
EmailStatusType = Literal[
    "Failed",
    "NotSent",
    "Sent",
]
```
## ErrorCodeType

```python
# ErrorCodeType usage example
from types_aiobotocore_chime.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "AccessDenied"
```

```python
# ErrorCodeType definition
ErrorCodeType = Literal[
    "AccessDenied",
    "BadRequest",
    "Conflict",
    "Forbidden",
    "NotFound",
    "PhoneNumberAssociationsExist",
    "PreconditionFailed",
    "ResourceLimitExceeded",
    "ServiceFailure",
    "ServiceUnavailable",
    "Throttled",
    "Throttling",
    "Unauthorized",
    "Unprocessable",
    "VoiceConnectorGroupAssociationsExist",
]
```
## GeoMatchLevelType

```python
# GeoMatchLevelType usage example
from types_aiobotocore_chime.literals import GeoMatchLevelType

def get_value() -> GeoMatchLevelType:
    return "AreaCode"
```

```python
# GeoMatchLevelType definition
GeoMatchLevelType = Literal[
    "AreaCode",
    "Country",
]
```
## InviteStatusType

```python
# InviteStatusType usage example
from types_aiobotocore_chime.literals import InviteStatusType

def get_value() -> InviteStatusType:
    return "Accepted"
```

```python
# InviteStatusType definition
InviteStatusType = Literal[
    "Accepted",
    "Failed",
    "Pending",
]
```
## LicenseType

```python
# LicenseType usage example
from types_aiobotocore_chime.literals import LicenseType

def get_value() -> LicenseType:
    return "Basic"
```

```python
# LicenseType definition
LicenseType = Literal[
    "Basic",
    "Plus",
    "Pro",
    "ProTrial",
]
```
## ListAccountsPaginatorName

```python
# ListAccountsPaginatorName usage example
from types_aiobotocore_chime.literals import ListAccountsPaginatorName

def get_value() -> ListAccountsPaginatorName:
    return "list_accounts"
```

```python
# ListAccountsPaginatorName definition
ListAccountsPaginatorName = Literal[
    "list_accounts",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example
from types_aiobotocore_chime.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition
ListUsersPaginatorName = Literal[
    "list_users",
]
```
## MediaPipelineSinkTypeType

```python
# MediaPipelineSinkTypeType usage example
from types_aiobotocore_chime.literals import MediaPipelineSinkTypeType

def get_value() -> MediaPipelineSinkTypeType:
    return "S3Bucket"
```

```python
# MediaPipelineSinkTypeType definition
MediaPipelineSinkTypeType = Literal[
    "S3Bucket",
]
```
## MediaPipelineSourceTypeType

```python
# MediaPipelineSourceTypeType usage example
from types_aiobotocore_chime.literals import MediaPipelineSourceTypeType

def get_value() -> MediaPipelineSourceTypeType:
    return "ChimeSdkMeeting"
```

```python
# MediaPipelineSourceTypeType definition
MediaPipelineSourceTypeType = Literal[
    "ChimeSdkMeeting",
]
```
## MediaPipelineStatusType

```python
# MediaPipelineStatusType usage example
from types_aiobotocore_chime.literals import MediaPipelineStatusType

def get_value() -> MediaPipelineStatusType:
    return "Failed"
```

```python
# MediaPipelineStatusType definition
MediaPipelineStatusType = Literal[
    "Failed",
    "Initializing",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## MemberTypeType

```python
# MemberTypeType usage example
from types_aiobotocore_chime.literals import MemberTypeType

def get_value() -> MemberTypeType:
    return "Bot"
```

```python
# MemberTypeType definition
MemberTypeType = Literal[
    "Bot",
    "User",
    "Webhook",
]
```
## NotificationTargetType

```python
# NotificationTargetType usage example
from types_aiobotocore_chime.literals import NotificationTargetType

def get_value() -> NotificationTargetType:
    return "EventBridge"
```

```python
# NotificationTargetType definition
NotificationTargetType = Literal[
    "EventBridge",
    "SNS",
    "SQS",
]
```
## NumberSelectionBehaviorType

```python
# NumberSelectionBehaviorType usage example
from types_aiobotocore_chime.literals import NumberSelectionBehaviorType

def get_value() -> NumberSelectionBehaviorType:
    return "AvoidSticky"
```

```python
# NumberSelectionBehaviorType definition
NumberSelectionBehaviorType = Literal[
    "AvoidSticky",
    "PreferSticky",
]
```
## OrderedPhoneNumberStatusType

```python
# OrderedPhoneNumberStatusType usage example
from types_aiobotocore_chime.literals import OrderedPhoneNumberStatusType

def get_value() -> OrderedPhoneNumberStatusType:
    return "Acquired"
```

```python
# OrderedPhoneNumberStatusType definition
OrderedPhoneNumberStatusType = Literal[
    "Acquired",
    "Failed",
    "Processing",
]
```
## OriginationRouteProtocolType

```python
# OriginationRouteProtocolType usage example
from types_aiobotocore_chime.literals import OriginationRouteProtocolType

def get_value() -> OriginationRouteProtocolType:
    return "TCP"
```

```python
# OriginationRouteProtocolType definition
OriginationRouteProtocolType = Literal[
    "TCP",
    "UDP",
]
```
## PhoneNumberAssociationNameType

```python
# PhoneNumberAssociationNameType usage example
from types_aiobotocore_chime.literals import PhoneNumberAssociationNameType

def get_value() -> PhoneNumberAssociationNameType:
    return "AccountId"
```

```python
# PhoneNumberAssociationNameType definition
PhoneNumberAssociationNameType = Literal[
    "AccountId",
    "SipRuleId",
    "UserId",
    "VoiceConnectorGroupId",
    "VoiceConnectorId",
]
```
## PhoneNumberOrderStatusType

```python
# PhoneNumberOrderStatusType usage example
from types_aiobotocore_chime.literals import PhoneNumberOrderStatusType

def get_value() -> PhoneNumberOrderStatusType:
    return "Failed"
```

```python
# PhoneNumberOrderStatusType definition
PhoneNumberOrderStatusType = Literal[
    "Failed",
    "Partial",
    "Processing",
    "Successful",
]
```
## PhoneNumberProductTypeType

```python
# PhoneNumberProductTypeType usage example
from types_aiobotocore_chime.literals import PhoneNumberProductTypeType

def get_value() -> PhoneNumberProductTypeType:
    return "BusinessCalling"
```

```python
# PhoneNumberProductTypeType definition
PhoneNumberProductTypeType = Literal[
    "BusinessCalling",
    "SipMediaApplicationDialIn",
    "VoiceConnector",
]
```
## PhoneNumberStatusType

```python
# PhoneNumberStatusType usage example
from types_aiobotocore_chime.literals import PhoneNumberStatusType

def get_value() -> PhoneNumberStatusType:
    return "AcquireFailed"
```

```python
# PhoneNumberStatusType definition
PhoneNumberStatusType = Literal[
    "AcquireFailed",
    "AcquireInProgress",
    "Assigned",
    "DeleteFailed",
    "DeleteInProgress",
    "ReleaseFailed",
    "ReleaseInProgress",
    "Unassigned",
]
```
## PhoneNumberTypeType

```python
# PhoneNumberTypeType usage example
from types_aiobotocore_chime.literals import PhoneNumberTypeType

def get_value() -> PhoneNumberTypeType:
    return "Local"
```

```python
# PhoneNumberTypeType definition
PhoneNumberTypeType = Literal[
    "Local",
    "TollFree",
]
```
## ProxySessionStatusType

```python
# ProxySessionStatusType usage example
from types_aiobotocore_chime.literals import ProxySessionStatusType

def get_value() -> ProxySessionStatusType:
    return "Closed"
```

```python
# ProxySessionStatusType definition
ProxySessionStatusType = Literal[
    "Closed",
    "InProgress",
    "Open",
]
```
## RegistrationStatusType

```python
# RegistrationStatusType usage example
from types_aiobotocore_chime.literals import RegistrationStatusType

def get_value() -> RegistrationStatusType:
    return "Registered"
```

```python
# RegistrationStatusType definition
RegistrationStatusType = Literal[
    "Registered",
    "Suspended",
    "Unregistered",
]
```
## RoomMembershipRoleType

```python
# RoomMembershipRoleType usage example
from types_aiobotocore_chime.literals import RoomMembershipRoleType

def get_value() -> RoomMembershipRoleType:
    return "Administrator"
```

```python
# RoomMembershipRoleType definition
RoomMembershipRoleType = Literal[
    "Administrator",
    "Member",
]
```
## SipRuleTriggerTypeType

```python
# SipRuleTriggerTypeType usage example
from types_aiobotocore_chime.literals import SipRuleTriggerTypeType

def get_value() -> SipRuleTriggerTypeType:
    return "RequestUriHostname"
```

```python
# SipRuleTriggerTypeType definition
SipRuleTriggerTypeType = Literal[
    "RequestUriHostname",
    "ToPhoneNumber",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_chime.literals import SortOrderType

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
## TranscribeContentIdentificationTypeType

```python
# TranscribeContentIdentificationTypeType usage example
from types_aiobotocore_chime.literals import TranscribeContentIdentificationTypeType

def get_value() -> TranscribeContentIdentificationTypeType:
    return "PII"
```

```python
# TranscribeContentIdentificationTypeType definition
TranscribeContentIdentificationTypeType = Literal[
    "PII",
]
```
## TranscribeContentRedactionTypeType

```python
# TranscribeContentRedactionTypeType usage example
from types_aiobotocore_chime.literals import TranscribeContentRedactionTypeType

def get_value() -> TranscribeContentRedactionTypeType:
    return "PII"
```

```python
# TranscribeContentRedactionTypeType definition
TranscribeContentRedactionTypeType = Literal[
    "PII",
]
```
## TranscribeLanguageCodeType

```python
# TranscribeLanguageCodeType usage example
from types_aiobotocore_chime.literals import TranscribeLanguageCodeType

def get_value() -> TranscribeLanguageCodeType:
    return "de-DE"
```

```python
# TranscribeLanguageCodeType definition
TranscribeLanguageCodeType = Literal[
    "de-DE",
    "en-AU",
    "en-GB",
    "en-US",
    "es-US",
    "fr-CA",
    "fr-FR",
    "hi-IN",
    "it-IT",
    "ja-JP",
    "ko-KR",
    "pt-BR",
    "th-TH",
    "zh-CN",
]
```
## TranscribeMedicalContentIdentificationTypeType

```python
# TranscribeMedicalContentIdentificationTypeType usage example
from types_aiobotocore_chime.literals import TranscribeMedicalContentIdentificationTypeType

def get_value() -> TranscribeMedicalContentIdentificationTypeType:
    return "PHI"
```

```python
# TranscribeMedicalContentIdentificationTypeType definition
TranscribeMedicalContentIdentificationTypeType = Literal[
    "PHI",
]
```
## TranscribeMedicalLanguageCodeType

```python
# TranscribeMedicalLanguageCodeType usage example
from types_aiobotocore_chime.literals import TranscribeMedicalLanguageCodeType

def get_value() -> TranscribeMedicalLanguageCodeType:
    return "en-US"
```

```python
# TranscribeMedicalLanguageCodeType definition
TranscribeMedicalLanguageCodeType = Literal[
    "en-US",
]
```
## TranscribeMedicalRegionType

```python
# TranscribeMedicalRegionType usage example
from types_aiobotocore_chime.literals import TranscribeMedicalRegionType

def get_value() -> TranscribeMedicalRegionType:
    return "ap-southeast-2"
```

```python
# TranscribeMedicalRegionType definition
TranscribeMedicalRegionType = Literal[
    "ap-southeast-2",
    "auto",
    "ca-central-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
## TranscribeMedicalSpecialtyType

```python
# TranscribeMedicalSpecialtyType usage example
from types_aiobotocore_chime.literals import TranscribeMedicalSpecialtyType

def get_value() -> TranscribeMedicalSpecialtyType:
    return "CARDIOLOGY"
```

```python
# TranscribeMedicalSpecialtyType definition
TranscribeMedicalSpecialtyType = Literal[
    "CARDIOLOGY",
    "NEUROLOGY",
    "ONCOLOGY",
    "PRIMARYCARE",
    "RADIOLOGY",
    "UROLOGY",
]
```
## TranscribeMedicalTypeType

```python
# TranscribeMedicalTypeType usage example
from types_aiobotocore_chime.literals import TranscribeMedicalTypeType

def get_value() -> TranscribeMedicalTypeType:
    return "CONVERSATION"
```

```python
# TranscribeMedicalTypeType definition
TranscribeMedicalTypeType = Literal[
    "CONVERSATION",
    "DICTATION",
]
```
## TranscribePartialResultsStabilityType

```python
# TranscribePartialResultsStabilityType usage example
from types_aiobotocore_chime.literals import TranscribePartialResultsStabilityType

def get_value() -> TranscribePartialResultsStabilityType:
    return "high"
```

```python
# TranscribePartialResultsStabilityType definition
TranscribePartialResultsStabilityType = Literal[
    "high",
    "low",
    "medium",
]
```
## TranscribeRegionType

```python
# TranscribeRegionType usage example
from types_aiobotocore_chime.literals import TranscribeRegionType

def get_value() -> TranscribeRegionType:
    return "ap-northeast-1"
```

```python
# TranscribeRegionType definition
TranscribeRegionType = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-southeast-2",
    "auto",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
## TranscribeVocabularyFilterMethodType

```python
# TranscribeVocabularyFilterMethodType usage example
from types_aiobotocore_chime.literals import TranscribeVocabularyFilterMethodType

def get_value() -> TranscribeVocabularyFilterMethodType:
    return "mask"
```

```python
# TranscribeVocabularyFilterMethodType definition
TranscribeVocabularyFilterMethodType = Literal[
    "mask",
    "remove",
    "tag",
]
```
## UserTypeType

```python
# UserTypeType usage example
from types_aiobotocore_chime.literals import UserTypeType

def get_value() -> UserTypeType:
    return "PrivateUser"
```

```python
# UserTypeType definition
UserTypeType = Literal[
    "PrivateUser",
    "SharedDevice",
]
```
## VideoMuxTypeType

```python
# VideoMuxTypeType usage example
from types_aiobotocore_chime.literals import VideoMuxTypeType

def get_value() -> VideoMuxTypeType:
    return "VideoOnly"
```

```python
# VideoMuxTypeType definition
VideoMuxTypeType = Literal[
    "VideoOnly",
]
```
## VoiceConnectorAwsRegionType

```python
# VoiceConnectorAwsRegionType usage example
from types_aiobotocore_chime.literals import VoiceConnectorAwsRegionType

def get_value() -> VoiceConnectorAwsRegionType:
    return "us-east-1"
```

```python
# VoiceConnectorAwsRegionType definition
VoiceConnectorAwsRegionType = Literal[
    "us-east-1",
    "us-west-2",
]
```
## ChimeServiceName

```python
# ChimeServiceName usage example
from types_aiobotocore_chime.literals import ChimeServiceName

def get_value() -> ChimeServiceName:
    return "chime"
```

```python
# ChimeServiceName definition
ChimeServiceName = Literal[
    "chime",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_chime.literals import ServiceName

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
    "apptest",
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
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
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
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
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
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
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
    "lookoutmetrics",
    "lookoutvision",
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
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "oam",
    "observabilityadmin",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
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
    "privatenetworks",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "qldb",
    "qldb-session",
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
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53profiles",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
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
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
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
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_chime.literals import ResourceServiceName

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
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_chime.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_accounts"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_accounts",
    "list_users",
]
```
