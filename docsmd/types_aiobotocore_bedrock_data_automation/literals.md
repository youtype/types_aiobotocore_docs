# Literals

> [Index](../README.md) > [DataAutomationforBedrock](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation](https://pypi.org/project/types-aiobotocore-bedrock-data-automation/).

## AudioExtractionCategoryTypeType

```python
# AudioExtractionCategoryTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import AudioExtractionCategoryTypeType

def get_value() -> AudioExtractionCategoryTypeType:
    return "AUDIO_CONTENT_MODERATION"
```

```python
# AudioExtractionCategoryTypeType definition

AudioExtractionCategoryTypeType = Literal[
    "AUDIO_CONTENT_MODERATION",
    "CHAPTER_CONTENT_MODERATION",
    "TRANSCRIPT",
]
```
## AudioStandardGenerativeFieldTypeType

```python
# AudioStandardGenerativeFieldTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import AudioStandardGenerativeFieldTypeType

def get_value() -> AudioStandardGenerativeFieldTypeType:
    return "AUDIO_SUMMARY"
```

```python
# AudioStandardGenerativeFieldTypeType definition

AudioStandardGenerativeFieldTypeType = Literal[
    "AUDIO_SUMMARY",
    "CHAPTER_SUMMARY",
    "IAB",
]
```
## BlueprintStageFilterType

```python
# BlueprintStageFilterType usage example

from types_aiobotocore_bedrock_data_automation.literals import BlueprintStageFilterType

def get_value() -> BlueprintStageFilterType:
    return "ALL"
```

```python
# BlueprintStageFilterType definition

BlueprintStageFilterType = Literal[
    "ALL",
    "DEVELOPMENT",
    "LIVE",
]
```
## BlueprintStageType

```python
# BlueprintStageType usage example

from types_aiobotocore_bedrock_data_automation.literals import BlueprintStageType

def get_value() -> BlueprintStageType:
    return "DEVELOPMENT"
```

```python
# BlueprintStageType definition

BlueprintStageType = Literal[
    "DEVELOPMENT",
    "LIVE",
]
```
## DataAutomationProjectStageFilterType

```python
# DataAutomationProjectStageFilterType usage example

from types_aiobotocore_bedrock_data_automation.literals import DataAutomationProjectStageFilterType

def get_value() -> DataAutomationProjectStageFilterType:
    return "ALL"
```

```python
# DataAutomationProjectStageFilterType definition

DataAutomationProjectStageFilterType = Literal[
    "ALL",
    "DEVELOPMENT",
    "LIVE",
]
```
## DataAutomationProjectStageType

```python
# DataAutomationProjectStageType usage example

from types_aiobotocore_bedrock_data_automation.literals import DataAutomationProjectStageType

def get_value() -> DataAutomationProjectStageType:
    return "DEVELOPMENT"
```

```python
# DataAutomationProjectStageType definition

DataAutomationProjectStageType = Literal[
    "DEVELOPMENT",
    "LIVE",
]
```
## DataAutomationProjectStatusType

```python
# DataAutomationProjectStatusType usage example

from types_aiobotocore_bedrock_data_automation.literals import DataAutomationProjectStatusType

def get_value() -> DataAutomationProjectStatusType:
    return "COMPLETED"
```

```python
# DataAutomationProjectStatusType definition

DataAutomationProjectStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## DocumentExtractionGranularityTypeType

```python
# DocumentExtractionGranularityTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import DocumentExtractionGranularityTypeType

def get_value() -> DocumentExtractionGranularityTypeType:
    return "DOCUMENT"
```

```python
# DocumentExtractionGranularityTypeType definition

DocumentExtractionGranularityTypeType = Literal[
    "DOCUMENT",
    "ELEMENT",
    "LINE",
    "PAGE",
    "WORD",
]
```
## DocumentOutputTextFormatTypeType

```python
# DocumentOutputTextFormatTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import DocumentOutputTextFormatTypeType

def get_value() -> DocumentOutputTextFormatTypeType:
    return "CSV"
```

```python
# DocumentOutputTextFormatTypeType definition

DocumentOutputTextFormatTypeType = Literal[
    "CSV",
    "HTML",
    "MARKDOWN",
    "PLAIN_TEXT",
]
```
## ImageExtractionCategoryTypeType

```python
# ImageExtractionCategoryTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import ImageExtractionCategoryTypeType

def get_value() -> ImageExtractionCategoryTypeType:
    return "CONTENT_MODERATION"
```

```python
# ImageExtractionCategoryTypeType definition

ImageExtractionCategoryTypeType = Literal[
    "CONTENT_MODERATION",
    "TEXT_DETECTION",
]
```
## ImageStandardGenerativeFieldTypeType

```python
# ImageStandardGenerativeFieldTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import ImageStandardGenerativeFieldTypeType

def get_value() -> ImageStandardGenerativeFieldTypeType:
    return "IAB"
```

```python
# ImageStandardGenerativeFieldTypeType definition

ImageStandardGenerativeFieldTypeType = Literal[
    "IAB",
    "IMAGE_SUMMARY",
]
```
## ListBlueprintsPaginatorName

```python
# ListBlueprintsPaginatorName usage example

from types_aiobotocore_bedrock_data_automation.literals import ListBlueprintsPaginatorName

def get_value() -> ListBlueprintsPaginatorName:
    return "list_blueprints"
```

```python
# ListBlueprintsPaginatorName definition

ListBlueprintsPaginatorName = Literal[
    "list_blueprints",
]
```
## ListDataAutomationProjectsPaginatorName

```python
# ListDataAutomationProjectsPaginatorName usage example

from types_aiobotocore_bedrock_data_automation.literals import ListDataAutomationProjectsPaginatorName

def get_value() -> ListDataAutomationProjectsPaginatorName:
    return "list_data_automation_projects"
```

```python
# ListDataAutomationProjectsPaginatorName definition

ListDataAutomationProjectsPaginatorName = Literal[
    "list_data_automation_projects",
]
```
## ResourceOwnerType

```python
# ResourceOwnerType usage example

from types_aiobotocore_bedrock_data_automation.literals import ResourceOwnerType

def get_value() -> ResourceOwnerType:
    return "ACCOUNT"
```

```python
# ResourceOwnerType definition

ResourceOwnerType = Literal[
    "ACCOUNT",
    "SERVICE",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_bedrock_data_automation.literals import StateType

def get_value() -> StateType:
    return "DISABLED"
```

```python
# StateType definition

StateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## TypeType

```python
# TypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import TypeType

def get_value() -> TypeType:
    return "DOCUMENT"
```

```python
# TypeType definition

TypeType = Literal[
    "DOCUMENT",
    "IMAGE",
]
```
## VideoExtractionCategoryTypeType

```python
# VideoExtractionCategoryTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import VideoExtractionCategoryTypeType

def get_value() -> VideoExtractionCategoryTypeType:
    return "CONTENT_MODERATION"
```

```python
# VideoExtractionCategoryTypeType definition

VideoExtractionCategoryTypeType = Literal[
    "CONTENT_MODERATION",
    "TEXT_DETECTION",
    "TRANSCRIPT",
]
```
## VideoStandardGenerativeFieldTypeType

```python
# VideoStandardGenerativeFieldTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import VideoStandardGenerativeFieldTypeType

def get_value() -> VideoStandardGenerativeFieldTypeType:
    return "IAB"
```

```python
# VideoStandardGenerativeFieldTypeType definition

VideoStandardGenerativeFieldTypeType = Literal[
    "IAB",
    "SCENE_SUMMARY",
    "VIDEO_SUMMARY",
]
```
## DataAutomationforBedrockServiceName

```python
# DataAutomationforBedrockServiceName usage example

from types_aiobotocore_bedrock_data_automation.literals import DataAutomationforBedrockServiceName

def get_value() -> DataAutomationforBedrockServiceName:
    return "bedrock-data-automation"
```

```python
# DataAutomationforBedrockServiceName definition

DataAutomationforBedrockServiceName = Literal[
    "bedrock-data-automation",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_bedrock_data_automation.literals import ServiceName

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

from types_aiobotocore_bedrock_data_automation.literals import ResourceServiceName

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

from types_aiobotocore_bedrock_data_automation.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_blueprints"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_blueprints",
    "list_data_automation_projects",
]
```
