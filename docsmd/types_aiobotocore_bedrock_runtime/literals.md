# Literals

> [Index](../README.md) > [BedrockRuntime](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## AsyncInvokeStatusType

```python
# AsyncInvokeStatusType usage example

from types_aiobotocore_bedrock_runtime.literals import AsyncInvokeStatusType

def get_value() -> AsyncInvokeStatusType:
    return "Completed"
```

```python
# AsyncInvokeStatusType definition

AsyncInvokeStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
]
```
## ConversationRoleType

```python
# ConversationRoleType usage example

from types_aiobotocore_bedrock_runtime.literals import ConversationRoleType

def get_value() -> ConversationRoleType:
    return "assistant"
```

```python
# ConversationRoleType definition

ConversationRoleType = Literal[
    "assistant",
    "user",
]
```
## DocumentFormatType

```python
# DocumentFormatType usage example

from types_aiobotocore_bedrock_runtime.literals import DocumentFormatType

def get_value() -> DocumentFormatType:
    return "csv"
```

```python
# DocumentFormatType definition

DocumentFormatType = Literal[
    "csv",
    "doc",
    "docx",
    "html",
    "md",
    "pdf",
    "txt",
    "xls",
    "xlsx",
]
```
## GuardrailActionType

```python
# GuardrailActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailActionType

def get_value() -> GuardrailActionType:
    return "GUARDRAIL_INTERVENED"
```

```python
# GuardrailActionType definition

GuardrailActionType = Literal[
    "GUARDRAIL_INTERVENED",
    "NONE",
]
```
## GuardrailContentFilterConfidenceType

```python
# GuardrailContentFilterConfidenceType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentFilterConfidenceType

def get_value() -> GuardrailContentFilterConfidenceType:
    return "HIGH"
```

```python
# GuardrailContentFilterConfidenceType definition

GuardrailContentFilterConfidenceType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
    "NONE",
]
```
## GuardrailContentFilterStrengthType

```python
# GuardrailContentFilterStrengthType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentFilterStrengthType

def get_value() -> GuardrailContentFilterStrengthType:
    return "HIGH"
```

```python
# GuardrailContentFilterStrengthType definition

GuardrailContentFilterStrengthType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
    "NONE",
]
```
## GuardrailContentFilterTypeType

```python
# GuardrailContentFilterTypeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentFilterTypeType

def get_value() -> GuardrailContentFilterTypeType:
    return "HATE"
```

```python
# GuardrailContentFilterTypeType definition

GuardrailContentFilterTypeType = Literal[
    "HATE",
    "INSULTS",
    "MISCONDUCT",
    "PROMPT_ATTACK",
    "SEXUAL",
    "VIOLENCE",
]
```
## GuardrailContentPolicyActionType

```python
# GuardrailContentPolicyActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentPolicyActionType

def get_value() -> GuardrailContentPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailContentPolicyActionType definition

GuardrailContentPolicyActionType = Literal[
    "BLOCKED",
]
```
## GuardrailContentQualifierType

```python
# GuardrailContentQualifierType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentQualifierType

def get_value() -> GuardrailContentQualifierType:
    return "grounding_source"
```

```python
# GuardrailContentQualifierType definition

GuardrailContentQualifierType = Literal[
    "grounding_source",
    "guard_content",
    "query",
]
```
## GuardrailContentSourceType

```python
# GuardrailContentSourceType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContentSourceType

def get_value() -> GuardrailContentSourceType:
    return "INPUT"
```

```python
# GuardrailContentSourceType definition

GuardrailContentSourceType = Literal[
    "INPUT",
    "OUTPUT",
]
```
## GuardrailContextualGroundingFilterTypeType

```python
# GuardrailContextualGroundingFilterTypeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContextualGroundingFilterTypeType

def get_value() -> GuardrailContextualGroundingFilterTypeType:
    return "GROUNDING"
```

```python
# GuardrailContextualGroundingFilterTypeType definition

GuardrailContextualGroundingFilterTypeType = Literal[
    "GROUNDING",
    "RELEVANCE",
]
```
## GuardrailContextualGroundingPolicyActionType

```python
# GuardrailContextualGroundingPolicyActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailContextualGroundingPolicyActionType

def get_value() -> GuardrailContextualGroundingPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailContextualGroundingPolicyActionType definition

GuardrailContextualGroundingPolicyActionType = Literal[
    "BLOCKED",
    "NONE",
]
```
## GuardrailConverseContentQualifierType

```python
# GuardrailConverseContentQualifierType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailConverseContentQualifierType

def get_value() -> GuardrailConverseContentQualifierType:
    return "grounding_source"
```

```python
# GuardrailConverseContentQualifierType definition

GuardrailConverseContentQualifierType = Literal[
    "grounding_source",
    "guard_content",
    "query",
]
```
## GuardrailConverseImageFormatType

```python
# GuardrailConverseImageFormatType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailConverseImageFormatType

def get_value() -> GuardrailConverseImageFormatType:
    return "jpeg"
```

```python
# GuardrailConverseImageFormatType definition

GuardrailConverseImageFormatType = Literal[
    "jpeg",
    "png",
]
```
## GuardrailImageFormatType

```python
# GuardrailImageFormatType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailImageFormatType

def get_value() -> GuardrailImageFormatType:
    return "jpeg"
```

```python
# GuardrailImageFormatType definition

GuardrailImageFormatType = Literal[
    "jpeg",
    "png",
]
```
## GuardrailManagedWordTypeType

```python
# GuardrailManagedWordTypeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailManagedWordTypeType

def get_value() -> GuardrailManagedWordTypeType:
    return "PROFANITY"
```

```python
# GuardrailManagedWordTypeType definition

GuardrailManagedWordTypeType = Literal[
    "PROFANITY",
]
```
## GuardrailPiiEntityTypeType

```python
# GuardrailPiiEntityTypeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailPiiEntityTypeType

def get_value() -> GuardrailPiiEntityTypeType:
    return "ADDRESS"
```

```python
# GuardrailPiiEntityTypeType definition

GuardrailPiiEntityTypeType = Literal[
    "ADDRESS",
    "AGE",
    "AWS_ACCESS_KEY",
    "AWS_SECRET_KEY",
    "CA_HEALTH_NUMBER",
    "CA_SOCIAL_INSURANCE_NUMBER",
    "CREDIT_DEBIT_CARD_CVV",
    "CREDIT_DEBIT_CARD_EXPIRY",
    "CREDIT_DEBIT_CARD_NUMBER",
    "DRIVER_ID",
    "EMAIL",
    "INTERNATIONAL_BANK_ACCOUNT_NUMBER",
    "IP_ADDRESS",
    "LICENSE_PLATE",
    "MAC_ADDRESS",
    "NAME",
    "PASSWORD",
    "PHONE",
    "PIN",
    "SWIFT_CODE",
    "UK_NATIONAL_HEALTH_SERVICE_NUMBER",
    "UK_NATIONAL_INSURANCE_NUMBER",
    "UK_UNIQUE_TAXPAYER_REFERENCE_NUMBER",
    "URL",
    "US_BANK_ACCOUNT_NUMBER",
    "US_BANK_ROUTING_NUMBER",
    "US_INDIVIDUAL_TAX_IDENTIFICATION_NUMBER",
    "US_PASSPORT_NUMBER",
    "US_SOCIAL_SECURITY_NUMBER",
    "USERNAME",
    "VEHICLE_IDENTIFICATION_NUMBER",
]
```
## GuardrailSensitiveInformationPolicyActionType

```python
# GuardrailSensitiveInformationPolicyActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailSensitiveInformationPolicyActionType

def get_value() -> GuardrailSensitiveInformationPolicyActionType:
    return "ANONYMIZED"
```

```python
# GuardrailSensitiveInformationPolicyActionType definition

GuardrailSensitiveInformationPolicyActionType = Literal[
    "ANONYMIZED",
    "BLOCKED",
]
```
## GuardrailStreamProcessingModeType

```python
# GuardrailStreamProcessingModeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailStreamProcessingModeType

def get_value() -> GuardrailStreamProcessingModeType:
    return "async"
```

```python
# GuardrailStreamProcessingModeType definition

GuardrailStreamProcessingModeType = Literal[
    "async",
    "sync",
]
```
## GuardrailTopicPolicyActionType

```python
# GuardrailTopicPolicyActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailTopicPolicyActionType

def get_value() -> GuardrailTopicPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailTopicPolicyActionType definition

GuardrailTopicPolicyActionType = Literal[
    "BLOCKED",
]
```
## GuardrailTopicTypeType

```python
# GuardrailTopicTypeType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailTopicTypeType

def get_value() -> GuardrailTopicTypeType:
    return "DENY"
```

```python
# GuardrailTopicTypeType definition

GuardrailTopicTypeType = Literal[
    "DENY",
]
```
## GuardrailTraceType

```python
# GuardrailTraceType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailTraceType

def get_value() -> GuardrailTraceType:
    return "disabled"
```

```python
# GuardrailTraceType definition

GuardrailTraceType = Literal[
    "disabled",
    "enabled",
]
```
## GuardrailWordPolicyActionType

```python
# GuardrailWordPolicyActionType usage example

from types_aiobotocore_bedrock_runtime.literals import GuardrailWordPolicyActionType

def get_value() -> GuardrailWordPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailWordPolicyActionType definition

GuardrailWordPolicyActionType = Literal[
    "BLOCKED",
]
```
## ImageFormatType

```python
# ImageFormatType usage example

from types_aiobotocore_bedrock_runtime.literals import ImageFormatType

def get_value() -> ImageFormatType:
    return "gif"
```

```python
# ImageFormatType definition

ImageFormatType = Literal[
    "gif",
    "jpeg",
    "png",
    "webp",
]
```
## ListAsyncInvokesPaginatorName

```python
# ListAsyncInvokesPaginatorName usage example

from types_aiobotocore_bedrock_runtime.literals import ListAsyncInvokesPaginatorName

def get_value() -> ListAsyncInvokesPaginatorName:
    return "list_async_invokes"
```

```python
# ListAsyncInvokesPaginatorName definition

ListAsyncInvokesPaginatorName = Literal[
    "list_async_invokes",
]
```
## PerformanceConfigLatencyType

```python
# PerformanceConfigLatencyType usage example

from types_aiobotocore_bedrock_runtime.literals import PerformanceConfigLatencyType

def get_value() -> PerformanceConfigLatencyType:
    return "optimized"
```

```python
# PerformanceConfigLatencyType definition

PerformanceConfigLatencyType = Literal[
    "optimized",
    "standard",
]
```
## SortAsyncInvocationByType

```python
# SortAsyncInvocationByType usage example

from types_aiobotocore_bedrock_runtime.literals import SortAsyncInvocationByType

def get_value() -> SortAsyncInvocationByType:
    return "SubmissionTime"
```

```python
# SortAsyncInvocationByType definition

SortAsyncInvocationByType = Literal[
    "SubmissionTime",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_bedrock_runtime.literals import SortOrderType

def get_value() -> SortOrderType:
    return "Ascending"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "Ascending",
    "Descending",
]
```
## StopReasonType

```python
# StopReasonType usage example

from types_aiobotocore_bedrock_runtime.literals import StopReasonType

def get_value() -> StopReasonType:
    return "content_filtered"
```

```python
# StopReasonType definition

StopReasonType = Literal[
    "content_filtered",
    "end_turn",
    "guardrail_intervened",
    "max_tokens",
    "stop_sequence",
    "tool_use",
]
```
## ToolResultStatusType

```python
# ToolResultStatusType usage example

from types_aiobotocore_bedrock_runtime.literals import ToolResultStatusType

def get_value() -> ToolResultStatusType:
    return "error"
```

```python
# ToolResultStatusType definition

ToolResultStatusType = Literal[
    "error",
    "success",
]
```
## TraceType

```python
# TraceType usage example

from types_aiobotocore_bedrock_runtime.literals import TraceType

def get_value() -> TraceType:
    return "DISABLED"
```

```python
# TraceType definition

TraceType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## VideoFormatType

```python
# VideoFormatType usage example

from types_aiobotocore_bedrock_runtime.literals import VideoFormatType

def get_value() -> VideoFormatType:
    return "flv"
```

```python
# VideoFormatType definition

VideoFormatType = Literal[
    "flv",
    "mkv",
    "mov",
    "mp4",
    "mpeg",
    "mpg",
    "three_gp",
    "webm",
    "wmv",
]
```
## BedrockRuntimeServiceName

```python
# BedrockRuntimeServiceName usage example

from types_aiobotocore_bedrock_runtime.literals import BedrockRuntimeServiceName

def get_value() -> BedrockRuntimeServiceName:
    return "bedrock-runtime"
```

```python
# BedrockRuntimeServiceName definition

BedrockRuntimeServiceName = Literal[
    "bedrock-runtime",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_bedrock_runtime.literals import ServiceName

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

from types_aiobotocore_bedrock_runtime.literals import ResourceServiceName

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

from types_aiobotocore_bedrock_runtime.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_async_invokes"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_async_invokes",
]
```
