# Literals

> [Index](../README.md) > [LookoutEquipment](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## DataUploadFrequencyType

```python
# DataUploadFrequencyType usage example

from types_aiobotocore_lookoutequipment.literals import DataUploadFrequencyType

def get_value() -> DataUploadFrequencyType:
    return "PT10M"
```

```python
# DataUploadFrequencyType definition

DataUploadFrequencyType = Literal[
    "PT10M",
    "PT15M",
    "PT1H",
    "PT30M",
    "PT5M",
]
```
## DatasetStatusType

```python
# DatasetStatusType usage example

from types_aiobotocore_lookoutequipment.literals import DatasetStatusType

def get_value() -> DatasetStatusType:
    return "ACTIVE"
```

```python
# DatasetStatusType definition

DatasetStatusType = Literal[
    "ACTIVE",
    "CREATED",
    "IMPORT_IN_PROGRESS",
    "INGESTION_IN_PROGRESS",
]
```
## InferenceExecutionStatusType

```python
# InferenceExecutionStatusType usage example

from types_aiobotocore_lookoutequipment.literals import InferenceExecutionStatusType

def get_value() -> InferenceExecutionStatusType:
    return "FAILED"
```

```python
# InferenceExecutionStatusType definition

InferenceExecutionStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## InferenceSchedulerStatusType

```python
# InferenceSchedulerStatusType usage example

from types_aiobotocore_lookoutequipment.literals import InferenceSchedulerStatusType

def get_value() -> InferenceSchedulerStatusType:
    return "PENDING"
```

```python
# InferenceSchedulerStatusType definition

InferenceSchedulerStatusType = Literal[
    "PENDING",
    "RUNNING",
    "STOPPED",
    "STOPPING",
]
```
## IngestionJobStatusType

```python
# IngestionJobStatusType usage example

from types_aiobotocore_lookoutequipment.literals import IngestionJobStatusType

def get_value() -> IngestionJobStatusType:
    return "FAILED"
```

```python
# IngestionJobStatusType definition

IngestionJobStatusType = Literal[
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## LabelRatingType

```python
# LabelRatingType usage example

from types_aiobotocore_lookoutequipment.literals import LabelRatingType

def get_value() -> LabelRatingType:
    return "ANOMALY"
```

```python
# LabelRatingType definition

LabelRatingType = Literal[
    "ANOMALY",
    "NEUTRAL",
    "NO_ANOMALY",
]
```
## LatestInferenceResultType

```python
# LatestInferenceResultType usage example

from types_aiobotocore_lookoutequipment.literals import LatestInferenceResultType

def get_value() -> LatestInferenceResultType:
    return "ANOMALOUS"
```

```python
# LatestInferenceResultType definition

LatestInferenceResultType = Literal[
    "ANOMALOUS",
    "NORMAL",
]
```
## ModelStatusType

```python
# ModelStatusType usage example

from types_aiobotocore_lookoutequipment.literals import ModelStatusType

def get_value() -> ModelStatusType:
    return "FAILED"
```

```python
# ModelStatusType definition

ModelStatusType = Literal[
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## ModelVersionSourceTypeType

```python
# ModelVersionSourceTypeType usage example

from types_aiobotocore_lookoutequipment.literals import ModelVersionSourceTypeType

def get_value() -> ModelVersionSourceTypeType:
    return "IMPORT"
```

```python
# ModelVersionSourceTypeType definition

ModelVersionSourceTypeType = Literal[
    "IMPORT",
    "RETRAINING",
    "TRAINING",
]
```
## ModelVersionStatusType

```python
# ModelVersionStatusType usage example

from types_aiobotocore_lookoutequipment.literals import ModelVersionStatusType

def get_value() -> ModelVersionStatusType:
    return "CANCELED"
```

```python
# ModelVersionStatusType definition

ModelVersionStatusType = Literal[
    "CANCELED",
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## MonotonicityType

```python
# MonotonicityType usage example

from types_aiobotocore_lookoutequipment.literals import MonotonicityType

def get_value() -> MonotonicityType:
    return "DECREASING"
```

```python
# MonotonicityType definition

MonotonicityType = Literal[
    "DECREASING",
    "INCREASING",
    "STATIC",
]
```
## StatisticalIssueStatusType

```python
# StatisticalIssueStatusType usage example

from types_aiobotocore_lookoutequipment.literals import StatisticalIssueStatusType

def get_value() -> StatisticalIssueStatusType:
    return "NO_ISSUE_DETECTED"
```

```python
# StatisticalIssueStatusType definition

StatisticalIssueStatusType = Literal[
    "NO_ISSUE_DETECTED",
    "POTENTIAL_ISSUE_DETECTED",
]
```
## TargetSamplingRateType

```python
# TargetSamplingRateType usage example

from types_aiobotocore_lookoutequipment.literals import TargetSamplingRateType

def get_value() -> TargetSamplingRateType:
    return "PT10M"
```

```python
# TargetSamplingRateType definition

TargetSamplingRateType = Literal[
    "PT10M",
    "PT10S",
    "PT15M",
    "PT15S",
    "PT1H",
    "PT1M",
    "PT1S",
    "PT30M",
    "PT30S",
    "PT5M",
    "PT5S",
]
```
## LookoutEquipmentServiceName

```python
# LookoutEquipmentServiceName usage example

from types_aiobotocore_lookoutequipment.literals import LookoutEquipmentServiceName

def get_value() -> LookoutEquipmentServiceName:
    return "lookoutequipment"
```

```python
# LookoutEquipmentServiceName definition

LookoutEquipmentServiceName = Literal[
    "lookoutequipment",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_lookoutequipment.literals import ServiceName

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

from types_aiobotocore_lookoutequipment.literals import ResourceServiceName

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

from types_aiobotocore_lookoutequipment.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-2"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-2",
    "eu-west-1",
    "us-east-1",
]
```
