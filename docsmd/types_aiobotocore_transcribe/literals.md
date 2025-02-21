# Literals

> [Index](../README.md) > [TranscribeService](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#transcribeservice)
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
## CallAnalyticsFeatureType

```python
# CallAnalyticsFeatureType usage example
from types_aiobotocore_transcribe.literals import CallAnalyticsFeatureType

def get_value() -> CallAnalyticsFeatureType:
    return "GENERATIVE_SUMMARIZATION"
```

```python
# CallAnalyticsFeatureType definition
CallAnalyticsFeatureType = Literal[
    "GENERATIVE_SUMMARIZATION",
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
## CallAnalyticsSkippedReasonCodeType

```python
# CallAnalyticsSkippedReasonCodeType usage example
from types_aiobotocore_transcribe.literals import CallAnalyticsSkippedReasonCodeType

def get_value() -> CallAnalyticsSkippedReasonCodeType:
    return "FAILED_SAFETY_GUIDELINES"
```

```python
# CallAnalyticsSkippedReasonCodeType definition
CallAnalyticsSkippedReasonCodeType = Literal[
    "FAILED_SAFETY_GUIDELINES",
    "INSUFFICIENT_CONVERSATION_CONTENT",
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
    return "ab-GE"
```

```python
# LanguageCodeType definition
LanguageCodeType = Literal[
    "ab-GE",
    "af-ZA",
    "ar-AE",
    "ar-SA",
    "ast-ES",
    "az-AZ",
    "ba-RU",
    "be-BY",
    "bg-BG",
    "bn-IN",
    "bs-BA",
    "ca-ES",
    "ckb-IQ",
    "ckb-IR",
    "cs-CZ",
    "cy-WL",
    "da-DK",
    "de-CH",
    "de-DE",
    "el-GR",
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
    "et-ET",
    "eu-ES",
    "fa-IR",
    "fi-FI",
    "fr-CA",
    "fr-FR",
    "gl-ES",
    "gu-IN",
    "ha-NG",
    "he-IL",
    "hi-IN",
    "hr-HR",
    "hu-HU",
    "hy-AM",
    "id-ID",
    "is-IS",
    "it-IT",
    "ja-JP",
    "ka-GE",
    "kab-DZ",
    "kk-KZ",
    "kn-IN",
    "ko-KR",
    "ky-KG",
    "lg-IN",
    "lt-LT",
    "lv-LV",
    "mhr-RU",
    "mi-NZ",
    "mk-MK",
    "ml-IN",
    "mn-MN",
    "mr-IN",
    "ms-MY",
    "mt-MT",
    "nl-NL",
    "no-NO",
    "or-IN",
    "pa-IN",
    "pl-PL",
    "ps-AF",
    "pt-BR",
    "pt-PT",
    "ro-RO",
    "ru-RU",
    "rw-RW",
    "si-LK",
    "sk-SK",
    "sl-SI",
    "so-SO",
    "sr-RS",
    "su-ID",
    "sv-SE",
    "sw-BI",
    "sw-KE",
    "sw-RW",
    "sw-TZ",
    "sw-UG",
    "ta-IN",
    "te-IN",
    "th-TH",
    "tl-PH",
    "tr-TR",
    "tt-RU",
    "ug-CN",
    "uk-UA",
    "uz-UZ",
    "vi-VN",
    "wo-SN",
    "zh-CN",
    "zh-TW",
    "zu-ZA",
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
    "m4a",
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
## MedicalScribeJobStatusType

```python
# MedicalScribeJobStatusType usage example
from types_aiobotocore_transcribe.literals import MedicalScribeJobStatusType

def get_value() -> MedicalScribeJobStatusType:
    return "COMPLETED"
```

```python
# MedicalScribeJobStatusType definition
MedicalScribeJobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "QUEUED",
]
```
## MedicalScribeLanguageCodeType

```python
# MedicalScribeLanguageCodeType usage example
from types_aiobotocore_transcribe.literals import MedicalScribeLanguageCodeType

def get_value() -> MedicalScribeLanguageCodeType:
    return "en-US"
```

```python
# MedicalScribeLanguageCodeType definition
MedicalScribeLanguageCodeType = Literal[
    "en-US",
]
```
## MedicalScribeNoteTemplateType

```python
# MedicalScribeNoteTemplateType usage example
from types_aiobotocore_transcribe.literals import MedicalScribeNoteTemplateType

def get_value() -> MedicalScribeNoteTemplateType:
    return "GIRPP"
```

```python
# MedicalScribeNoteTemplateType definition
MedicalScribeNoteTemplateType = Literal[
    "GIRPP",
    "HISTORY_AND_PHYSICAL",
]
```
## MedicalScribeParticipantRoleType

```python
# MedicalScribeParticipantRoleType usage example
from types_aiobotocore_transcribe.literals import MedicalScribeParticipantRoleType

def get_value() -> MedicalScribeParticipantRoleType:
    return "CLINICIAN"
```

```python
# MedicalScribeParticipantRoleType definition
MedicalScribeParticipantRoleType = Literal[
    "CLINICIAN",
    "PATIENT",
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
