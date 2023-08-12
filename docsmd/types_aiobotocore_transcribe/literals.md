# Literals

> [Index](../README.md) > [TranscribeService](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
    type annotations stubs module [types-aiobotocore-transcribe](https://pypi.org/project/types-aiobotocore-transcribe/).

## BaseModelNameType

```python
# BaseModelNameType usage example

from types_aiobotocore_transcribe.literals import BaseModelNameType

def get_value() -> BaseModelNameType:
    return "NarrowBand"
```

```python
# BaseModelNameType definition

BaseModelNameType = Literal[
    "NarrowBand",
    "WideBand",
]
```
## CLMLanguageCodeType

```python
# CLMLanguageCodeType usage example

from types_aiobotocore_transcribe.literals import CLMLanguageCodeType

def get_value() -> CLMLanguageCodeType:
    return "de-DE"
```

```python
# CLMLanguageCodeType definition

CLMLanguageCodeType = Literal[
    "de-DE",
    "en-AU",
    "en-GB",
    "en-US",
    "es-US",
    "hi-IN",
    "ja-JP",
]
```
## CallAnalyticsJobStatusType

```python
# CallAnalyticsJobStatusType usage example

from types_aiobotocore_transcribe.literals import CallAnalyticsJobStatusType

def get_value() -> CallAnalyticsJobStatusType:
    return "COMPLETED"
```

```python
# CallAnalyticsJobStatusType definition

CallAnalyticsJobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "QUEUED",
]
```
## InputTypeType

```python
# InputTypeType usage example

from types_aiobotocore_transcribe.literals import InputTypeType

def get_value() -> InputTypeType:
    return "POST_CALL"
```

```python
# InputTypeType definition

InputTypeType = Literal[
    "POST_CALL",
    "REAL_TIME",
]
```
## LanguageCodeType

```python
# LanguageCodeType usage example

from types_aiobotocore_transcribe.literals import LanguageCodeType

def get_value() -> LanguageCodeType:
    return "af-ZA"
```

```python
# LanguageCodeType definition

LanguageCodeType = Literal[
    "af-ZA",
    "ar-AE",
    "ar-SA",
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
    "fa-IR",
    "fr-CA",
    "fr-FR",
    "he-IL",
    "hi-IN",
    "id-ID",
    "it-IT",
    "ja-JP",
    "ko-KR",
    "ms-MY",
    "nl-NL",
    "pt-BR",
    "pt-PT",
    "ru-RU",
    "sv-SE",
    "ta-IN",
    "te-IN",
    "th-TH",
    "tr-TR",
    "vi-VN",
    "zh-CN",
    "zh-TW",
]
```
## MediaFormatType

```python
# MediaFormatType usage example

from types_aiobotocore_transcribe.literals import MediaFormatType

def get_value() -> MediaFormatType:
    return "amr"
```

```python
# MediaFormatType definition

MediaFormatType = Literal[
    "amr",
    "flac",
    "mp3",
    "mp4",
    "ogg",
    "wav",
    "webm",
]
```
## MedicalContentIdentificationTypeType

```python
# MedicalContentIdentificationTypeType usage example

from types_aiobotocore_transcribe.literals import MedicalContentIdentificationTypeType

def get_value() -> MedicalContentIdentificationTypeType:
    return "PHI"
```

```python
# MedicalContentIdentificationTypeType definition

MedicalContentIdentificationTypeType = Literal[
    "PHI",
]
```
## ModelStatusType

```python
# ModelStatusType usage example

from types_aiobotocore_transcribe.literals import ModelStatusType

def get_value() -> ModelStatusType:
    return "COMPLETED"
```

```python
# ModelStatusType definition

ModelStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## OutputLocationTypeType

```python
# OutputLocationTypeType usage example

from types_aiobotocore_transcribe.literals import OutputLocationTypeType

def get_value() -> OutputLocationTypeType:
    return "CUSTOMER_BUCKET"
```

```python
# OutputLocationTypeType definition

OutputLocationTypeType = Literal[
    "CUSTOMER_BUCKET",
    "SERVICE_BUCKET",
]
```
## ParticipantRoleType

```python
# ParticipantRoleType usage example

from types_aiobotocore_transcribe.literals import ParticipantRoleType

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
## PiiEntityTypeType

```python
# PiiEntityTypeType usage example

from types_aiobotocore_transcribe.literals import PiiEntityTypeType

def get_value() -> PiiEntityTypeType:
    return "ADDRESS"
```

```python
# PiiEntityTypeType definition

PiiEntityTypeType = Literal[
    "ADDRESS",
    "ALL",
    "BANK_ACCOUNT_NUMBER",
    "BANK_ROUTING",
    "CREDIT_DEBIT_CVV",
    "CREDIT_DEBIT_EXPIRY",
    "CREDIT_DEBIT_NUMBER",
    "EMAIL",
    "NAME",
    "PHONE",
    "PIN",
    "SSN",
]
```
## RedactionOutputType

```python
# RedactionOutputType usage example

from types_aiobotocore_transcribe.literals import RedactionOutputType

def get_value() -> RedactionOutputType:
    return "redacted"
```

```python
# RedactionOutputType definition

RedactionOutputType = Literal[
    "redacted",
    "redacted_and_unredacted",
]
```
## RedactionTypeType

```python
# RedactionTypeType usage example

from types_aiobotocore_transcribe.literals import RedactionTypeType

def get_value() -> RedactionTypeType:
    return "PII"
```

```python
# RedactionTypeType definition

RedactionTypeType = Literal[
    "PII",
]
```
## SentimentValueType

```python
# SentimentValueType usage example

from types_aiobotocore_transcribe.literals import SentimentValueType

def get_value() -> SentimentValueType:
    return "MIXED"
```

```python
# SentimentValueType definition

SentimentValueType = Literal[
    "MIXED",
    "NEGATIVE",
    "NEUTRAL",
    "POSITIVE",
]
```
## SpecialtyType

```python
# SpecialtyType usage example

from types_aiobotocore_transcribe.literals import SpecialtyType

def get_value() -> SpecialtyType:
    return "PRIMARYCARE"
```

```python
# SpecialtyType definition

SpecialtyType = Literal[
    "PRIMARYCARE",
]
```
## SubtitleFormatType

```python
# SubtitleFormatType usage example

from types_aiobotocore_transcribe.literals import SubtitleFormatType

def get_value() -> SubtitleFormatType:
    return "srt"
```

```python
# SubtitleFormatType definition

SubtitleFormatType = Literal[
    "srt",
    "vtt",
]
```
## ToxicityCategoryType

```python
# ToxicityCategoryType usage example

from types_aiobotocore_transcribe.literals import ToxicityCategoryType

def get_value() -> ToxicityCategoryType:
    return "ALL"
```

```python
# ToxicityCategoryType definition

ToxicityCategoryType = Literal[
    "ALL",
]
```
## TranscriptFilterTypeType

```python
# TranscriptFilterTypeType usage example

from types_aiobotocore_transcribe.literals import TranscriptFilterTypeType

def get_value() -> TranscriptFilterTypeType:
    return "EXACT"
```

```python
# TranscriptFilterTypeType definition

TranscriptFilterTypeType = Literal[
    "EXACT",
]
```
## TranscriptionJobStatusType

```python
# TranscriptionJobStatusType usage example

from types_aiobotocore_transcribe.literals import TranscriptionJobStatusType

def get_value() -> TranscriptionJobStatusType:
    return "COMPLETED"
```

```python
# TranscriptionJobStatusType definition

TranscriptionJobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "QUEUED",
]
```
## TypeType

```python
# TypeType usage example

from types_aiobotocore_transcribe.literals import TypeType

def get_value() -> TypeType:
    return "CONVERSATION"
```

```python
# TypeType definition

TypeType = Literal[
    "CONVERSATION",
    "DICTATION",
]
```
## VocabularyFilterMethodType

```python
# VocabularyFilterMethodType usage example

from types_aiobotocore_transcribe.literals import VocabularyFilterMethodType

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
## VocabularyStateType

```python
# VocabularyStateType usage example

from types_aiobotocore_transcribe.literals import VocabularyStateType

def get_value() -> VocabularyStateType:
    return "FAILED"
```

```python
# VocabularyStateType definition

VocabularyStateType = Literal[
    "FAILED",
    "PENDING",
    "READY",
]
```
## TranscribeServiceServiceName

```python
# TranscribeServiceServiceName usage example

from types_aiobotocore_transcribe.literals import TranscribeServiceServiceName

def get_value() -> TranscribeServiceServiceName:
    return "transcribe"
```

```python
# TranscribeServiceServiceName definition

TranscribeServiceServiceName = Literal[
    "transcribe",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_transcribe.literals import ServiceName

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

from types_aiobotocore_transcribe.literals import ResourceServiceName

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

from types_aiobotocore_transcribe.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
