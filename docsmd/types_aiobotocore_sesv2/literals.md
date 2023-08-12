# Literals

> [Index](../README.md) > [SESV2](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## BehaviorOnMxFailureType

```python
# BehaviorOnMxFailureType usage example

from types_aiobotocore_sesv2.literals import BehaviorOnMxFailureType

def get_value() -> BehaviorOnMxFailureType:
    return "REJECT_MESSAGE"
```

```python
# BehaviorOnMxFailureType definition

BehaviorOnMxFailureType = Literal[
    "REJECT_MESSAGE",
    "USE_DEFAULT_VALUE",
]
```
## BulkEmailStatusType

```python
# BulkEmailStatusType usage example

from types_aiobotocore_sesv2.literals import BulkEmailStatusType

def get_value() -> BulkEmailStatusType:
    return "ACCOUNT_DAILY_QUOTA_EXCEEDED"
```

```python
# BulkEmailStatusType definition

BulkEmailStatusType = Literal[
    "ACCOUNT_DAILY_QUOTA_EXCEEDED",
    "ACCOUNT_SENDING_PAUSED",
    "ACCOUNT_SUSPENDED",
    "ACCOUNT_THROTTLED",
    "CONFIGURATION_SET_NOT_FOUND",
    "CONFIGURATION_SET_SENDING_PAUSED",
    "FAILED",
    "INVALID_PARAMETER",
    "INVALID_SENDING_POOL_NAME",
    "MAIL_FROM_DOMAIN_NOT_VERIFIED",
    "MESSAGE_REJECTED",
    "SUCCESS",
    "TEMPLATE_NOT_FOUND",
    "TRANSIENT_FAILURE",
]
```
## ContactLanguageType

```python
# ContactLanguageType usage example

from types_aiobotocore_sesv2.literals import ContactLanguageType

def get_value() -> ContactLanguageType:
    return "EN"
```

```python
# ContactLanguageType definition

ContactLanguageType = Literal[
    "EN",
    "JA",
]
```
## ContactListImportActionType

```python
# ContactListImportActionType usage example

from types_aiobotocore_sesv2.literals import ContactListImportActionType

def get_value() -> ContactListImportActionType:
    return "DELETE"
```

```python
# ContactListImportActionType definition

ContactListImportActionType = Literal[
    "DELETE",
    "PUT",
]
```
## DataFormatType

```python
# DataFormatType usage example

from types_aiobotocore_sesv2.literals import DataFormatType

def get_value() -> DataFormatType:
    return "CSV"
```

```python
# DataFormatType definition

DataFormatType = Literal[
    "CSV",
    "JSON",
]
```
## DeliverabilityDashboardAccountStatusType

```python
# DeliverabilityDashboardAccountStatusType usage example

from types_aiobotocore_sesv2.literals import DeliverabilityDashboardAccountStatusType

def get_value() -> DeliverabilityDashboardAccountStatusType:
    return "ACTIVE"
```

```python
# DeliverabilityDashboardAccountStatusType definition

DeliverabilityDashboardAccountStatusType = Literal[
    "ACTIVE",
    "DISABLED",
    "PENDING_EXPIRATION",
]
```
## DeliverabilityTestStatusType

```python
# DeliverabilityTestStatusType usage example

from types_aiobotocore_sesv2.literals import DeliverabilityTestStatusType

def get_value() -> DeliverabilityTestStatusType:
    return "COMPLETED"
```

```python
# DeliverabilityTestStatusType definition

DeliverabilityTestStatusType = Literal[
    "COMPLETED",
    "IN_PROGRESS",
]
```
## DimensionValueSourceType

```python
# DimensionValueSourceType usage example

from types_aiobotocore_sesv2.literals import DimensionValueSourceType

def get_value() -> DimensionValueSourceType:
    return "EMAIL_HEADER"
```

```python
# DimensionValueSourceType definition

DimensionValueSourceType = Literal[
    "EMAIL_HEADER",
    "LINK_TAG",
    "MESSAGE_TAG",
]
```
## DkimSigningAttributesOriginType

```python
# DkimSigningAttributesOriginType usage example

from types_aiobotocore_sesv2.literals import DkimSigningAttributesOriginType

def get_value() -> DkimSigningAttributesOriginType:
    return "AWS_SES"
```

```python
# DkimSigningAttributesOriginType definition

DkimSigningAttributesOriginType = Literal[
    "AWS_SES",
    "EXTERNAL",
]
```
## DkimSigningKeyLengthType

```python
# DkimSigningKeyLengthType usage example

from types_aiobotocore_sesv2.literals import DkimSigningKeyLengthType

def get_value() -> DkimSigningKeyLengthType:
    return "RSA_1024_BIT"
```

```python
# DkimSigningKeyLengthType definition

DkimSigningKeyLengthType = Literal[
    "RSA_1024_BIT",
    "RSA_2048_BIT",
]
```
## DkimStatusType

```python
# DkimStatusType usage example

from types_aiobotocore_sesv2.literals import DkimStatusType

def get_value() -> DkimStatusType:
    return "FAILED"
```

```python
# DkimStatusType definition

DkimStatusType = Literal[
    "FAILED",
    "NOT_STARTED",
    "PENDING",
    "SUCCESS",
    "TEMPORARY_FAILURE",
]
```
## EventTypeType

```python
# EventTypeType usage example

from types_aiobotocore_sesv2.literals import EventTypeType

def get_value() -> EventTypeType:
    return "BOUNCE"
```

```python
# EventTypeType definition

EventTypeType = Literal[
    "BOUNCE",
    "CLICK",
    "COMPLAINT",
    "DELIVERY",
    "DELIVERY_DELAY",
    "OPEN",
    "REJECT",
    "RENDERING_FAILURE",
    "SEND",
    "SUBSCRIPTION",
]
```
## FeatureStatusType

```python
# FeatureStatusType usage example

from types_aiobotocore_sesv2.literals import FeatureStatusType

def get_value() -> FeatureStatusType:
    return "DISABLED"
```

```python
# FeatureStatusType definition

FeatureStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## IdentityTypeType

```python
# IdentityTypeType usage example

from types_aiobotocore_sesv2.literals import IdentityTypeType

def get_value() -> IdentityTypeType:
    return "DOMAIN"
```

```python
# IdentityTypeType definition

IdentityTypeType = Literal[
    "DOMAIN",
    "EMAIL_ADDRESS",
    "MANAGED_DOMAIN",
]
```
## ImportDestinationTypeType

```python
# ImportDestinationTypeType usage example

from types_aiobotocore_sesv2.literals import ImportDestinationTypeType

def get_value() -> ImportDestinationTypeType:
    return "CONTACT_LIST"
```

```python
# ImportDestinationTypeType definition

ImportDestinationTypeType = Literal[
    "CONTACT_LIST",
    "SUPPRESSION_LIST",
]
```
## JobStatusType

```python
# JobStatusType usage example

from types_aiobotocore_sesv2.literals import JobStatusType

def get_value() -> JobStatusType:
    return "COMPLETED"
```

```python
# JobStatusType definition

JobStatusType = Literal[
    "COMPLETED",
    "CREATED",
    "FAILED",
    "PROCESSING",
]
```
## ListRecommendationsFilterKeyType

```python
# ListRecommendationsFilterKeyType usage example

from types_aiobotocore_sesv2.literals import ListRecommendationsFilterKeyType

def get_value() -> ListRecommendationsFilterKeyType:
    return "IMPACT"
```

```python
# ListRecommendationsFilterKeyType definition

ListRecommendationsFilterKeyType = Literal[
    "IMPACT",
    "RESOURCE_ARN",
    "STATUS",
    "TYPE",
]
```
## MailFromDomainStatusType

```python
# MailFromDomainStatusType usage example

from types_aiobotocore_sesv2.literals import MailFromDomainStatusType

def get_value() -> MailFromDomainStatusType:
    return "FAILED"
```

```python
# MailFromDomainStatusType definition

MailFromDomainStatusType = Literal[
    "FAILED",
    "PENDING",
    "SUCCESS",
    "TEMPORARY_FAILURE",
]
```
## MailTypeType

```python
# MailTypeType usage example

from types_aiobotocore_sesv2.literals import MailTypeType

def get_value() -> MailTypeType:
    return "MARKETING"
```

```python
# MailTypeType definition

MailTypeType = Literal[
    "MARKETING",
    "TRANSACTIONAL",
]
```
## MetricDimensionNameType

```python
# MetricDimensionNameType usage example

from types_aiobotocore_sesv2.literals import MetricDimensionNameType

def get_value() -> MetricDimensionNameType:
    return "CONFIGURATION_SET"
```

```python
# MetricDimensionNameType definition

MetricDimensionNameType = Literal[
    "CONFIGURATION_SET",
    "EMAIL_IDENTITY",
    "ISP",
]
```
## MetricNamespaceType

```python
# MetricNamespaceType usage example

from types_aiobotocore_sesv2.literals import MetricNamespaceType

def get_value() -> MetricNamespaceType:
    return "VDM"
```

```python
# MetricNamespaceType definition

MetricNamespaceType = Literal[
    "VDM",
]
```
## MetricType

```python
# MetricType usage example

from types_aiobotocore_sesv2.literals import MetricType

def get_value() -> MetricType:
    return "CLICK"
```

```python
# MetricType definition

MetricType = Literal[
    "CLICK",
    "COMPLAINT",
    "DELIVERY",
    "DELIVERY_CLICK",
    "DELIVERY_COMPLAINT",
    "DELIVERY_OPEN",
    "OPEN",
    "PERMANENT_BOUNCE",
    "SEND",
    "TRANSIENT_BOUNCE",
]
```
## QueryErrorCodeType

```python
# QueryErrorCodeType usage example

from types_aiobotocore_sesv2.literals import QueryErrorCodeType

def get_value() -> QueryErrorCodeType:
    return "ACCESS_DENIED"
```

```python
# QueryErrorCodeType definition

QueryErrorCodeType = Literal[
    "ACCESS_DENIED",
    "INTERNAL_FAILURE",
]
```
## RecommendationImpactType

```python
# RecommendationImpactType usage example

from types_aiobotocore_sesv2.literals import RecommendationImpactType

def get_value() -> RecommendationImpactType:
    return "HIGH"
```

```python
# RecommendationImpactType definition

RecommendationImpactType = Literal[
    "HIGH",
    "LOW",
]
```
## RecommendationStatusType

```python
# RecommendationStatusType usage example

from types_aiobotocore_sesv2.literals import RecommendationStatusType

def get_value() -> RecommendationStatusType:
    return "FIXED"
```

```python
# RecommendationStatusType definition

RecommendationStatusType = Literal[
    "FIXED",
    "OPEN",
]
```
## RecommendationTypeType

```python
# RecommendationTypeType usage example

from types_aiobotocore_sesv2.literals import RecommendationTypeType

def get_value() -> RecommendationTypeType:
    return "BIMI"
```

```python
# RecommendationTypeType definition

RecommendationTypeType = Literal[
    "BIMI",
    "DKIM",
    "DMARC",
    "SPF",
]
```
## ReviewStatusType

```python
# ReviewStatusType usage example

from types_aiobotocore_sesv2.literals import ReviewStatusType

def get_value() -> ReviewStatusType:
    return "DENIED"
```

```python
# ReviewStatusType definition

ReviewStatusType = Literal[
    "DENIED",
    "FAILED",
    "GRANTED",
    "PENDING",
]
```
## ScalingModeType

```python
# ScalingModeType usage example

from types_aiobotocore_sesv2.literals import ScalingModeType

def get_value() -> ScalingModeType:
    return "MANAGED"
```

```python
# ScalingModeType definition

ScalingModeType = Literal[
    "MANAGED",
    "STANDARD",
]
```
## SubscriptionStatusType

```python
# SubscriptionStatusType usage example

from types_aiobotocore_sesv2.literals import SubscriptionStatusType

def get_value() -> SubscriptionStatusType:
    return "OPT_IN"
```

```python
# SubscriptionStatusType definition

SubscriptionStatusType = Literal[
    "OPT_IN",
    "OPT_OUT",
]
```
## SuppressionListImportActionType

```python
# SuppressionListImportActionType usage example

from types_aiobotocore_sesv2.literals import SuppressionListImportActionType

def get_value() -> SuppressionListImportActionType:
    return "DELETE"
```

```python
# SuppressionListImportActionType definition

SuppressionListImportActionType = Literal[
    "DELETE",
    "PUT",
]
```
## SuppressionListReasonType

```python
# SuppressionListReasonType usage example

from types_aiobotocore_sesv2.literals import SuppressionListReasonType

def get_value() -> SuppressionListReasonType:
    return "BOUNCE"
```

```python
# SuppressionListReasonType definition

SuppressionListReasonType = Literal[
    "BOUNCE",
    "COMPLAINT",
]
```
## TlsPolicyType

```python
# TlsPolicyType usage example

from types_aiobotocore_sesv2.literals import TlsPolicyType

def get_value() -> TlsPolicyType:
    return "OPTIONAL"
```

```python
# TlsPolicyType definition

TlsPolicyType = Literal[
    "OPTIONAL",
    "REQUIRE",
]
```
## VerificationStatusType

```python
# VerificationStatusType usage example

from types_aiobotocore_sesv2.literals import VerificationStatusType

def get_value() -> VerificationStatusType:
    return "FAILED"
```

```python
# VerificationStatusType definition

VerificationStatusType = Literal[
    "FAILED",
    "NOT_STARTED",
    "PENDING",
    "SUCCESS",
    "TEMPORARY_FAILURE",
]
```
## WarmupStatusType

```python
# WarmupStatusType usage example

from types_aiobotocore_sesv2.literals import WarmupStatusType

def get_value() -> WarmupStatusType:
    return "DONE"
```

```python
# WarmupStatusType definition

WarmupStatusType = Literal[
    "DONE",
    "IN_PROGRESS",
]
```
## SESV2ServiceName

```python
# SESV2ServiceName usage example

from types_aiobotocore_sesv2.literals import SESV2ServiceName

def get_value() -> SESV2ServiceName:
    return "sesv2"
```

```python
# SESV2ServiceName definition

SESV2ServiceName = Literal[
    "sesv2",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_sesv2.literals import ServiceName

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

from types_aiobotocore_sesv2.literals import ResourceServiceName

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

from types_aiobotocore_sesv2.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
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
