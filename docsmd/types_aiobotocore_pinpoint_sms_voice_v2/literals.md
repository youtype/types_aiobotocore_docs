# Literals

> [Index](../README.md) > [PinpointSMSVoiceV2](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).

## AccountAttributeNameType

```python
# AccountAttributeNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import AccountAttributeNameType

def get_value() -> AccountAttributeNameType:
    return "ACCOUNT_TIER"
```

```python
# AccountAttributeNameType definition

AccountAttributeNameType = Literal[
    "ACCOUNT_TIER",
]
```
## AccountLimitNameType

```python
# AccountLimitNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import AccountLimitNameType

def get_value() -> AccountLimitNameType:
    return "CONFIGURATION_SETS"
```

```python
# AccountLimitNameType definition

AccountLimitNameType = Literal[
    "CONFIGURATION_SETS",
    "OPT_OUT_LISTS",
    "PHONE_NUMBERS",
    "POOLS",
]
```
## ConfigurationSetFilterNameType

```python
# ConfigurationSetFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import ConfigurationSetFilterNameType

def get_value() -> ConfigurationSetFilterNameType:
    return "default-message-type"
```

```python
# ConfigurationSetFilterNameType definition

ConfigurationSetFilterNameType = Literal[
    "default-message-type",
    "default-sender-id",
    "event-destination-name",
    "matching-event-types",
]
```
## DescribeAccountAttributesPaginatorName

```python
# DescribeAccountAttributesPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeAccountAttributesPaginatorName

def get_value() -> DescribeAccountAttributesPaginatorName:
    return "describe_account_attributes"
```

```python
# DescribeAccountAttributesPaginatorName definition

DescribeAccountAttributesPaginatorName = Literal[
    "describe_account_attributes",
]
```
## DescribeAccountLimitsPaginatorName

```python
# DescribeAccountLimitsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeAccountLimitsPaginatorName

def get_value() -> DescribeAccountLimitsPaginatorName:
    return "describe_account_limits"
```

```python
# DescribeAccountLimitsPaginatorName definition

DescribeAccountLimitsPaginatorName = Literal[
    "describe_account_limits",
]
```
## DescribeConfigurationSetsPaginatorName

```python
# DescribeConfigurationSetsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeConfigurationSetsPaginatorName

def get_value() -> DescribeConfigurationSetsPaginatorName:
    return "describe_configuration_sets"
```

```python
# DescribeConfigurationSetsPaginatorName definition

DescribeConfigurationSetsPaginatorName = Literal[
    "describe_configuration_sets",
]
```
## DescribeKeywordsPaginatorName

```python
# DescribeKeywordsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeKeywordsPaginatorName

def get_value() -> DescribeKeywordsPaginatorName:
    return "describe_keywords"
```

```python
# DescribeKeywordsPaginatorName definition

DescribeKeywordsPaginatorName = Literal[
    "describe_keywords",
]
```
## DescribeOptOutListsPaginatorName

```python
# DescribeOptOutListsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeOptOutListsPaginatorName

def get_value() -> DescribeOptOutListsPaginatorName:
    return "describe_opt_out_lists"
```

```python
# DescribeOptOutListsPaginatorName definition

DescribeOptOutListsPaginatorName = Literal[
    "describe_opt_out_lists",
]
```
## DescribeOptedOutNumbersPaginatorName

```python
# DescribeOptedOutNumbersPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeOptedOutNumbersPaginatorName

def get_value() -> DescribeOptedOutNumbersPaginatorName:
    return "describe_opted_out_numbers"
```

```python
# DescribeOptedOutNumbersPaginatorName definition

DescribeOptedOutNumbersPaginatorName = Literal[
    "describe_opted_out_numbers",
]
```
## DescribePhoneNumbersPaginatorName

```python
# DescribePhoneNumbersPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribePhoneNumbersPaginatorName

def get_value() -> DescribePhoneNumbersPaginatorName:
    return "describe_phone_numbers"
```

```python
# DescribePhoneNumbersPaginatorName definition

DescribePhoneNumbersPaginatorName = Literal[
    "describe_phone_numbers",
]
```
## DescribePoolsPaginatorName

```python
# DescribePoolsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribePoolsPaginatorName

def get_value() -> DescribePoolsPaginatorName:
    return "describe_pools"
```

```python
# DescribePoolsPaginatorName definition

DescribePoolsPaginatorName = Literal[
    "describe_pools",
]
```
## DescribeSenderIdsPaginatorName

```python
# DescribeSenderIdsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeSenderIdsPaginatorName

def get_value() -> DescribeSenderIdsPaginatorName:
    return "describe_sender_ids"
```

```python
# DescribeSenderIdsPaginatorName definition

DescribeSenderIdsPaginatorName = Literal[
    "describe_sender_ids",
]
```
## DescribeSpendLimitsPaginatorName

```python
# DescribeSpendLimitsPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DescribeSpendLimitsPaginatorName

def get_value() -> DescribeSpendLimitsPaginatorName:
    return "describe_spend_limits"
```

```python
# DescribeSpendLimitsPaginatorName definition

DescribeSpendLimitsPaginatorName = Literal[
    "describe_spend_limits",
]
```
## DestinationCountryParameterKeyType

```python
# DestinationCountryParameterKeyType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import DestinationCountryParameterKeyType

def get_value() -> DestinationCountryParameterKeyType:
    return "IN_ENTITY_ID"
```

```python
# DestinationCountryParameterKeyType definition

DestinationCountryParameterKeyType = Literal[
    "IN_ENTITY_ID",
    "IN_TEMPLATE_ID",
]
```
## EventTypeType

```python
# EventTypeType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import EventTypeType

def get_value() -> EventTypeType:
    return "ALL"
```

```python
# EventTypeType definition

EventTypeType = Literal[
    "ALL",
    "TEXT_ALL",
    "TEXT_BLOCKED",
    "TEXT_CARRIER_BLOCKED",
    "TEXT_CARRIER_UNREACHABLE",
    "TEXT_DELIVERED",
    "TEXT_INVALID",
    "TEXT_INVALID_MESSAGE",
    "TEXT_PENDING",
    "TEXT_QUEUED",
    "TEXT_SENT",
    "TEXT_SPAM",
    "TEXT_SUCCESSFUL",
    "TEXT_TTL_EXPIRED",
    "TEXT_UNKNOWN",
    "TEXT_UNREACHABLE",
    "VOICE_ALL",
    "VOICE_ANSWERED",
    "VOICE_BUSY",
    "VOICE_COMPLETED",
    "VOICE_FAILED",
    "VOICE_INITIATED",
    "VOICE_NO_ANSWER",
    "VOICE_RINGING",
    "VOICE_TTL_EXPIRED",
]
```
## KeywordActionType

```python
# KeywordActionType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import KeywordActionType

def get_value() -> KeywordActionType:
    return "AUTOMATIC_RESPONSE"
```

```python
# KeywordActionType definition

KeywordActionType = Literal[
    "AUTOMATIC_RESPONSE",
    "OPT_IN",
    "OPT_OUT",
]
```
## KeywordFilterNameType

```python
# KeywordFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import KeywordFilterNameType

def get_value() -> KeywordFilterNameType:
    return "keyword-action"
```

```python
# KeywordFilterNameType definition

KeywordFilterNameType = Literal[
    "keyword-action",
]
```
## ListPoolOriginationIdentitiesPaginatorName

```python
# ListPoolOriginationIdentitiesPaginatorName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import ListPoolOriginationIdentitiesPaginatorName

def get_value() -> ListPoolOriginationIdentitiesPaginatorName:
    return "list_pool_origination_identities"
```

```python
# ListPoolOriginationIdentitiesPaginatorName definition

ListPoolOriginationIdentitiesPaginatorName = Literal[
    "list_pool_origination_identities",
]
```
## MessageTypeType

```python
# MessageTypeType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import MessageTypeType

def get_value() -> MessageTypeType:
    return "PROMOTIONAL"
```

```python
# MessageTypeType definition

MessageTypeType = Literal[
    "PROMOTIONAL",
    "TRANSACTIONAL",
]
```
## NumberCapabilityType

```python
# NumberCapabilityType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import NumberCapabilityType

def get_value() -> NumberCapabilityType:
    return "SMS"
```

```python
# NumberCapabilityType definition

NumberCapabilityType = Literal[
    "SMS",
    "VOICE",
]
```
## NumberStatusType

```python
# NumberStatusType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import NumberStatusType

def get_value() -> NumberStatusType:
    return "ACTIVE"
```

```python
# NumberStatusType definition

NumberStatusType = Literal[
    "ACTIVE",
    "ASSOCIATING",
    "DELETED",
    "DISASSOCIATING",
    "PENDING",
]
```
## NumberTypeType

```python
# NumberTypeType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import NumberTypeType

def get_value() -> NumberTypeType:
    return "LONG_CODE"
```

```python
# NumberTypeType definition

NumberTypeType = Literal[
    "LONG_CODE",
    "SHORT_CODE",
    "TEN_DLC",
    "TOLL_FREE",
]
```
## OptedOutFilterNameType

```python
# OptedOutFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import OptedOutFilterNameType

def get_value() -> OptedOutFilterNameType:
    return "end-user-opted-out"
```

```python
# OptedOutFilterNameType definition

OptedOutFilterNameType = Literal[
    "end-user-opted-out",
]
```
## PhoneNumberFilterNameType

```python
# PhoneNumberFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PhoneNumberFilterNameType

def get_value() -> PhoneNumberFilterNameType:
    return "deletion-protection-enabled"
```

```python
# PhoneNumberFilterNameType definition

PhoneNumberFilterNameType = Literal[
    "deletion-protection-enabled",
    "iso-country-code",
    "message-type",
    "number-capability",
    "number-type",
    "opt-out-list-name",
    "self-managed-opt-outs-enabled",
    "status",
    "two-way-enabled",
]
```
## PoolFilterNameType

```python
# PoolFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PoolFilterNameType

def get_value() -> PoolFilterNameType:
    return "deletion-protection-enabled"
```

```python
# PoolFilterNameType definition

PoolFilterNameType = Literal[
    "deletion-protection-enabled",
    "message-type",
    "opt-out-list-name",
    "self-managed-opt-outs-enabled",
    "shared-routes-enabled",
    "status",
    "two-way-enabled",
]
```
## PoolOriginationIdentitiesFilterNameType

```python
# PoolOriginationIdentitiesFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PoolOriginationIdentitiesFilterNameType

def get_value() -> PoolOriginationIdentitiesFilterNameType:
    return "iso-country-code"
```

```python
# PoolOriginationIdentitiesFilterNameType definition

PoolOriginationIdentitiesFilterNameType = Literal[
    "iso-country-code",
    "number-capability",
]
```
## PoolStatusType

```python
# PoolStatusType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PoolStatusType

def get_value() -> PoolStatusType:
    return "ACTIVE"
```

```python
# PoolStatusType definition

PoolStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
]
```
## RequestableNumberTypeType

```python
# RequestableNumberTypeType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import RequestableNumberTypeType

def get_value() -> RequestableNumberTypeType:
    return "LONG_CODE"
```

```python
# RequestableNumberTypeType definition

RequestableNumberTypeType = Literal[
    "LONG_CODE",
    "TEN_DLC",
    "TOLL_FREE",
]
```
## SenderIdFilterNameType

```python
# SenderIdFilterNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import SenderIdFilterNameType

def get_value() -> SenderIdFilterNameType:
    return "iso-country-code"
```

```python
# SenderIdFilterNameType definition

SenderIdFilterNameType = Literal[
    "iso-country-code",
    "message-type",
    "sender-id",
]
```
## SpendLimitNameType

```python
# SpendLimitNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import SpendLimitNameType

def get_value() -> SpendLimitNameType:
    return "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT"
```

```python
# SpendLimitNameType definition

SpendLimitNameType = Literal[
    "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT",
    "VOICE_MESSAGE_MONTHLY_SPEND_LIMIT",
]
```
## VoiceIdType

```python
# VoiceIdType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import VoiceIdType

def get_value() -> VoiceIdType:
    return "AMY"
```

```python
# VoiceIdType definition

VoiceIdType = Literal[
    "AMY",
    "ASTRID",
    "BIANCA",
    "BRIAN",
    "CAMILA",
    "CARLA",
    "CARMEN",
    "CELINE",
    "CHANTAL",
    "CONCHITA",
    "CRISTIANO",
    "DORA",
    "EMMA",
    "ENRIQUE",
    "EWA",
    "FILIZ",
    "GERAINT",
    "GIORGIO",
    "GWYNETH",
    "HANS",
    "INES",
    "IVY",
    "JACEK",
    "JAN",
    "JOANNA",
    "JOEY",
    "JUSTIN",
    "KARL",
    "KENDRA",
    "KIMBERLY",
    "LEA",
    "LIV",
    "LOTTE",
    "LUCIA",
    "LUPE",
    "MADS",
    "MAJA",
    "MARLENE",
    "MATHIEU",
    "MATTHEW",
    "MAXIM",
    "MIA",
    "MIGUEL",
    "MIZUKI",
    "NAJA",
    "NICOLE",
    "PENELOPE",
    "RAVEENA",
    "RICARDO",
    "RUBEN",
    "RUSSELL",
    "SALLI",
    "SEOYEON",
    "TAKUMI",
    "TATYANA",
    "VICKI",
    "VITORIA",
    "ZEINA",
    "ZHIYU",
]
```
## VoiceMessageBodyTextTypeType

```python
# VoiceMessageBodyTextTypeType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import VoiceMessageBodyTextTypeType

def get_value() -> VoiceMessageBodyTextTypeType:
    return "SSML"
```

```python
# VoiceMessageBodyTextTypeType definition

VoiceMessageBodyTextTypeType = Literal[
    "SSML",
    "TEXT",
]
```
## PinpointSMSVoiceV2ServiceName

```python
# PinpointSMSVoiceV2ServiceName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PinpointSMSVoiceV2ServiceName

def get_value() -> PinpointSMSVoiceV2ServiceName:
    return "pinpoint-sms-voice-v2"
```

```python
# PinpointSMSVoiceV2ServiceName definition

PinpointSMSVoiceV2ServiceName = Literal[
    "pinpoint-sms-voice-v2",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import ServiceName

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

from types_aiobotocore_pinpoint_sms_voice_v2.literals import ResourceServiceName

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

from types_aiobotocore_pinpoint_sms_voice_v2.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_account_attributes"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_account_attributes",
    "describe_account_limits",
    "describe_configuration_sets",
    "describe_keywords",
    "describe_opt_out_lists",
    "describe_opted_out_numbers",
    "describe_phone_numbers",
    "describe_pools",
    "describe_sender_ids",
    "describe_spend_limits",
    "list_pool_origination_identities",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "us-east-1",
    "us-west-2",
]
```
