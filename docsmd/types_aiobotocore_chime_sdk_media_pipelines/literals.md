# Literals

> [Index](../README.md) > [ChimeSDKMediaPipelines](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## ActiveSpeakerPositionType

```python
# ActiveSpeakerPositionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType

def get_value() -> ActiveSpeakerPositionType:
    return "BottomLeft"
```

```python
# ActiveSpeakerPositionType definition

ActiveSpeakerPositionType = Literal[
    "BottomLeft",
    "BottomRight",
    "TopLeft",
    "TopRight",
]
```
## ArtifactsConcatenationStateType

```python
# ArtifactsConcatenationStateType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType

def get_value() -> ArtifactsConcatenationStateType:
    return "Disabled"
```

```python
# ArtifactsConcatenationStateType definition

ArtifactsConcatenationStateType = Literal[
    "Disabled",
    "Enabled",
]
```
## ArtifactsStateType

```python
# ArtifactsStateType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsStateType

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
## AudioArtifactsConcatenationStateType

```python
# AudioArtifactsConcatenationStateType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import AudioArtifactsConcatenationStateType

def get_value() -> AudioArtifactsConcatenationStateType:
    return "Enabled"
```

```python
# AudioArtifactsConcatenationStateType definition

AudioArtifactsConcatenationStateType = Literal[
    "Enabled",
]
```
## AudioChannelsOptionType

```python
# AudioChannelsOptionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import AudioChannelsOptionType

def get_value() -> AudioChannelsOptionType:
    return "Mono"
```

```python
# AudioChannelsOptionType definition

AudioChannelsOptionType = Literal[
    "Mono",
    "Stereo",
]
```
## AudioMuxTypeType

```python
# AudioMuxTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import AudioMuxTypeType

def get_value() -> AudioMuxTypeType:
    return "AudioOnly"
```

```python
# AudioMuxTypeType definition

AudioMuxTypeType = Literal[
    "AudioOnly",
    "AudioWithActiveSpeakerVideo",
    "AudioWithCompositedVideo",
]
```
## BorderColorType

```python
# BorderColorType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import BorderColorType

def get_value() -> BorderColorType:
    return "Black"
```

```python
# BorderColorType definition

BorderColorType = Literal[
    "Black",
    "Blue",
    "Green",
    "Red",
    "White",
    "Yellow",
]
```
## CallAnalyticsLanguageCodeType

```python
# CallAnalyticsLanguageCodeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import CallAnalyticsLanguageCodeType

def get_value() -> CallAnalyticsLanguageCodeType:
    return "de-DE"
```

```python
# CallAnalyticsLanguageCodeType definition

CallAnalyticsLanguageCodeType = Literal[
    "de-DE",
    "en-AU",
    "en-GB",
    "en-US",
    "es-US",
    "fr-CA",
    "fr-FR",
    "it-IT",
    "pt-BR",
]
```
## CanvasOrientationType

```python
# CanvasOrientationType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import CanvasOrientationType

def get_value() -> CanvasOrientationType:
    return "Landscape"
```

```python
# CanvasOrientationType definition

CanvasOrientationType = Literal[
    "Landscape",
    "Portrait",
]
```
## ConcatenationSinkTypeType

```python
# ConcatenationSinkTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ConcatenationSinkTypeType

def get_value() -> ConcatenationSinkTypeType:
    return "S3Bucket"
```

```python
# ConcatenationSinkTypeType definition

ConcatenationSinkTypeType = Literal[
    "S3Bucket",
]
```
## ConcatenationSourceTypeType

```python
# ConcatenationSourceTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ConcatenationSourceTypeType

def get_value() -> ConcatenationSourceTypeType:
    return "MediaCapturePipeline"
```

```python
# ConcatenationSourceTypeType definition

ConcatenationSourceTypeType = Literal[
    "MediaCapturePipeline",
]
```
## ContentMuxTypeType

```python
# ContentMuxTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ContentMuxTypeType

def get_value() -> ContentMuxTypeType:
    return "ContentOnly"
```

```python
# ContentMuxTypeType definition

ContentMuxTypeType = Literal[
    "ContentOnly",
]
```
## ContentRedactionOutputType

```python
# ContentRedactionOutputType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ContentRedactionOutputType

def get_value() -> ContentRedactionOutputType:
    return "redacted"
```

```python
# ContentRedactionOutputType definition

ContentRedactionOutputType = Literal[
    "redacted",
    "redacted_and_unredacted",
]
```
## ContentShareLayoutOptionType

```python
# ContentShareLayoutOptionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ContentShareLayoutOptionType

def get_value() -> ContentShareLayoutOptionType:
    return "ActiveSpeakerOnly"
```

```python
# ContentShareLayoutOptionType definition

ContentShareLayoutOptionType = Literal[
    "ActiveSpeakerOnly",
    "Horizontal",
    "PresenterOnly",
    "Vertical",
]
```
## ContentTypeType

```python
# ContentTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ContentTypeType

def get_value() -> ContentTypeType:
    return "PII"
```

```python
# ContentTypeType definition

ContentTypeType = Literal[
    "PII",
]
```
## FragmentSelectorTypeType

```python
# FragmentSelectorTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import FragmentSelectorTypeType

def get_value() -> FragmentSelectorTypeType:
    return "ProducerTimestamp"
```

```python
# FragmentSelectorTypeType definition

FragmentSelectorTypeType = Literal[
    "ProducerTimestamp",
    "ServerTimestamp",
]
```
## HighlightColorType

```python
# HighlightColorType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import HighlightColorType

def get_value() -> HighlightColorType:
    return "Black"
```

```python
# HighlightColorType definition

HighlightColorType = Literal[
    "Black",
    "Blue",
    "Green",
    "Red",
    "White",
    "Yellow",
]
```
## HorizontalTilePositionType

```python
# HorizontalTilePositionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import HorizontalTilePositionType

def get_value() -> HorizontalTilePositionType:
    return "Bottom"
```

```python
# HorizontalTilePositionType definition

HorizontalTilePositionType = Literal[
    "Bottom",
    "Top",
]
```
## LayoutOptionType

```python
# LayoutOptionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import LayoutOptionType

def get_value() -> LayoutOptionType:
    return "GridView"
```

```python
# LayoutOptionType definition

LayoutOptionType = Literal[
    "GridView",
]
```
## LiveConnectorMuxTypeType

```python
# LiveConnectorMuxTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import LiveConnectorMuxTypeType

def get_value() -> LiveConnectorMuxTypeType:
    return "AudioWithActiveSpeakerVideo"
```

```python
# LiveConnectorMuxTypeType definition

LiveConnectorMuxTypeType = Literal[
    "AudioWithActiveSpeakerVideo",
    "AudioWithCompositedVideo",
]
```
## LiveConnectorSinkTypeType

```python
# LiveConnectorSinkTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import LiveConnectorSinkTypeType

def get_value() -> LiveConnectorSinkTypeType:
    return "RTMP"
```

```python
# LiveConnectorSinkTypeType definition

LiveConnectorSinkTypeType = Literal[
    "RTMP",
]
```
## LiveConnectorSourceTypeType

```python
# LiveConnectorSourceTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import LiveConnectorSourceTypeType

def get_value() -> LiveConnectorSourceTypeType:
    return "ChimeSdkMeeting"
```

```python
# LiveConnectorSourceTypeType definition

LiveConnectorSourceTypeType = Literal[
    "ChimeSdkMeeting",
]
```
## MediaEncodingType

```python
# MediaEncodingType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaEncodingType

def get_value() -> MediaEncodingType:
    return "pcm"
```

```python
# MediaEncodingType definition

MediaEncodingType = Literal[
    "pcm",
]
```
## MediaInsightsPipelineConfigurationElementTypeType

```python
# MediaInsightsPipelineConfigurationElementTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaInsightsPipelineConfigurationElementTypeType

def get_value() -> MediaInsightsPipelineConfigurationElementTypeType:
    return "AmazonTranscribeCallAnalyticsProcessor"
```

```python
# MediaInsightsPipelineConfigurationElementTypeType definition

MediaInsightsPipelineConfigurationElementTypeType = Literal[
    "AmazonTranscribeCallAnalyticsProcessor",
    "AmazonTranscribeProcessor",
    "KinesisDataStreamSink",
    "LambdaFunctionSink",
    "S3RecordingSink",
    "SnsTopicSink",
    "SqsQueueSink",
    "VoiceAnalyticsProcessor",
]
```
## MediaPipelineSinkTypeType

```python
# MediaPipelineSinkTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaPipelineSinkTypeType

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

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaPipelineSourceTypeType

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

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaPipelineStatusType

def get_value() -> MediaPipelineStatusType:
    return "Failed"
```

```python
# MediaPipelineStatusType definition

MediaPipelineStatusType = Literal[
    "Failed",
    "Initializing",
    "InProgress",
    "Paused",
    "Stopped",
    "Stopping",
]
```
## MediaPipelineStatusUpdateType

```python
# MediaPipelineStatusUpdateType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import MediaPipelineStatusUpdateType

def get_value() -> MediaPipelineStatusUpdateType:
    return "Pause"
```

```python
# MediaPipelineStatusUpdateType definition

MediaPipelineStatusUpdateType = Literal[
    "Pause",
    "Resume",
]
```
## PartialResultsStabilityType

```python
# PartialResultsStabilityType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import PartialResultsStabilityType

def get_value() -> PartialResultsStabilityType:
    return "high"
```

```python
# PartialResultsStabilityType definition

PartialResultsStabilityType = Literal[
    "high",
    "low",
    "medium",
]
```
## ParticipantRoleType

```python
# ParticipantRoleType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ParticipantRoleType

def get_value() -> ParticipantRoleType:
    return "AGENT"
```

```python
# ParticipantRoleType definition

ParticipantRoleType = Literal[
    "AGENT",
    "CUSTOMER",
]
```
## PresenterPositionType

```python
# PresenterPositionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import PresenterPositionType

def get_value() -> PresenterPositionType:
    return "BottomLeft"
```

```python
# PresenterPositionType definition

PresenterPositionType = Literal[
    "BottomLeft",
    "BottomRight",
    "TopLeft",
    "TopRight",
]
```
## RealTimeAlertRuleTypeType

```python
# RealTimeAlertRuleTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import RealTimeAlertRuleTypeType

def get_value() -> RealTimeAlertRuleTypeType:
    return "IssueDetection"
```

```python
# RealTimeAlertRuleTypeType definition

RealTimeAlertRuleTypeType = Literal[
    "IssueDetection",
    "KeywordMatch",
    "Sentiment",
]
```
## RecordingFileFormatType

```python
# RecordingFileFormatType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import RecordingFileFormatType

def get_value() -> RecordingFileFormatType:
    return "Opus"
```

```python
# RecordingFileFormatType definition

RecordingFileFormatType = Literal[
    "Opus",
    "Wav",
]
```
## ResolutionOptionType

```python
# ResolutionOptionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ResolutionOptionType

def get_value() -> ResolutionOptionType:
    return "FHD"
```

```python
# ResolutionOptionType definition

ResolutionOptionType = Literal[
    "FHD",
    "HD",
]
```
## SentimentTypeType

```python
# SentimentTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import SentimentTypeType

def get_value() -> SentimentTypeType:
    return "NEGATIVE"
```

```python
# SentimentTypeType definition

SentimentTypeType = Literal[
    "NEGATIVE",
]
```
## TileOrderType

```python
# TileOrderType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import TileOrderType

def get_value() -> TileOrderType:
    return "JoinSequence"
```

```python
# TileOrderType definition

TileOrderType = Literal[
    "JoinSequence",
    "SpeakerSequence",
]
```
## VerticalTilePositionType

```python
# VerticalTilePositionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import VerticalTilePositionType

def get_value() -> VerticalTilePositionType:
    return "Left"
```

```python
# VerticalTilePositionType definition

VerticalTilePositionType = Literal[
    "Left",
    "Right",
]
```
## VideoMuxTypeType

```python
# VideoMuxTypeType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import VideoMuxTypeType

def get_value() -> VideoMuxTypeType:
    return "VideoOnly"
```

```python
# VideoMuxTypeType definition

VideoMuxTypeType = Literal[
    "VideoOnly",
]
```
## VocabularyFilterMethodType

```python
# VocabularyFilterMethodType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import VocabularyFilterMethodType

def get_value() -> VocabularyFilterMethodType:
    return "mask"
```

```python
# VocabularyFilterMethodType definition

VocabularyFilterMethodType = Literal[
    "mask",
    "remove",
    "tag",
]
```
## VoiceAnalyticsConfigurationStatusType

```python
# VoiceAnalyticsConfigurationStatusType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import VoiceAnalyticsConfigurationStatusType

def get_value() -> VoiceAnalyticsConfigurationStatusType:
    return "Disabled"
```

```python
# VoiceAnalyticsConfigurationStatusType definition

VoiceAnalyticsConfigurationStatusType = Literal[
    "Disabled",
    "Enabled",
]
```
## ChimeSDKMediaPipelinesServiceName

```python
# ChimeSDKMediaPipelinesServiceName usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ChimeSDKMediaPipelinesServiceName

def get_value() -> ChimeSDKMediaPipelinesServiceName:
    return "chime-sdk-media-pipelines"
```

```python
# ChimeSDKMediaPipelinesServiceName definition

ChimeSDKMediaPipelinesServiceName = Literal[
    "chime-sdk-media-pipelines",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ServiceName

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
    "alexaforbusiness",
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
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
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
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
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
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
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
    "fsx",
    "gamelift",
    "gamesparks",
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
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
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
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
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
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
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
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
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
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ResourceServiceName

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
## RegionName

```python
# RegionName usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import RegionName

def get_value() -> RegionName:
    return "ap-southeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-southeast-1",
    "eu-central-1",
    "us-east-1",
    "us-west-2",
]
```
