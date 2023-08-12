# Literals

> [Index](../README.md) > [imagebuilder](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## BuildTypeType

```python
# BuildTypeType usage example

from types_aiobotocore_imagebuilder.literals import BuildTypeType

def get_value() -> BuildTypeType:
    return "IMPORT"
```

```python
# BuildTypeType definition

BuildTypeType = Literal[
    "IMPORT",
    "SCHEDULED",
    "USER_INITIATED",
]
```
## ComponentFormatType

```python
# ComponentFormatType usage example

from types_aiobotocore_imagebuilder.literals import ComponentFormatType

def get_value() -> ComponentFormatType:
    return "SHELL"
```

```python
# ComponentFormatType definition

ComponentFormatType = Literal[
    "SHELL",
]
```
## ComponentStatusType

```python
# ComponentStatusType usage example

from types_aiobotocore_imagebuilder.literals import ComponentStatusType

def get_value() -> ComponentStatusType:
    return "DEPRECATED"
```

```python
# ComponentStatusType definition

ComponentStatusType = Literal[
    "DEPRECATED",
]
```
## ComponentTypeType

```python
# ComponentTypeType usage example

from types_aiobotocore_imagebuilder.literals import ComponentTypeType

def get_value() -> ComponentTypeType:
    return "BUILD"
```

```python
# ComponentTypeType definition

ComponentTypeType = Literal[
    "BUILD",
    "TEST",
]
```
## ContainerRepositoryServiceType

```python
# ContainerRepositoryServiceType usage example

from types_aiobotocore_imagebuilder.literals import ContainerRepositoryServiceType

def get_value() -> ContainerRepositoryServiceType:
    return "ECR"
```

```python
# ContainerRepositoryServiceType definition

ContainerRepositoryServiceType = Literal[
    "ECR",
]
```
## ContainerTypeType

```python
# ContainerTypeType usage example

from types_aiobotocore_imagebuilder.literals import ContainerTypeType

def get_value() -> ContainerTypeType:
    return "DOCKER"
```

```python
# ContainerTypeType definition

ContainerTypeType = Literal[
    "DOCKER",
]
```
## DiskImageFormatType

```python
# DiskImageFormatType usage example

from types_aiobotocore_imagebuilder.literals import DiskImageFormatType

def get_value() -> DiskImageFormatType:
    return "RAW"
```

```python
# DiskImageFormatType definition

DiskImageFormatType = Literal[
    "RAW",
    "VHD",
    "VMDK",
]
```
## EbsVolumeTypeType

```python
# EbsVolumeTypeType usage example

from types_aiobotocore_imagebuilder.literals import EbsVolumeTypeType

def get_value() -> EbsVolumeTypeType:
    return "gp2"
```

```python
# EbsVolumeTypeType definition

EbsVolumeTypeType = Literal[
    "gp2",
    "gp3",
    "io1",
    "io2",
    "sc1",
    "st1",
    "standard",
]
```
## ImageScanStatusType

```python
# ImageScanStatusType usage example

from types_aiobotocore_imagebuilder.literals import ImageScanStatusType

def get_value() -> ImageScanStatusType:
    return "ABANDONED"
```

```python
# ImageScanStatusType definition

ImageScanStatusType = Literal[
    "ABANDONED",
    "COLLECTING",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "SCANNING",
    "TIMED_OUT",
]
```
## ImageSourceType

```python
# ImageSourceType usage example

from types_aiobotocore_imagebuilder.literals import ImageSourceType

def get_value() -> ImageSourceType:
    return "AMAZON_MANAGED"
```

```python
# ImageSourceType definition

ImageSourceType = Literal[
    "AMAZON_MANAGED",
    "AWS_MARKETPLACE",
    "CUSTOM",
    "IMPORTED",
]
```
## ImageStatusType

```python
# ImageStatusType usage example

from types_aiobotocore_imagebuilder.literals import ImageStatusType

def get_value() -> ImageStatusType:
    return "AVAILABLE"
```

```python
# ImageStatusType definition

ImageStatusType = Literal[
    "AVAILABLE",
    "BUILDING",
    "CANCELLED",
    "CREATING",
    "DELETED",
    "DEPRECATED",
    "DISTRIBUTING",
    "FAILED",
    "INTEGRATING",
    "PENDING",
    "TESTING",
]
```
## ImageTypeType

```python
# ImageTypeType usage example

from types_aiobotocore_imagebuilder.literals import ImageTypeType

def get_value() -> ImageTypeType:
    return "AMI"
```

```python
# ImageTypeType definition

ImageTypeType = Literal[
    "AMI",
    "DOCKER",
]
```
## OwnershipType

```python
# OwnershipType usage example

from types_aiobotocore_imagebuilder.literals import OwnershipType

def get_value() -> OwnershipType:
    return "Amazon"
```

```python
# OwnershipType definition

OwnershipType = Literal[
    "Amazon",
    "Self",
    "Shared",
    "ThirdParty",
]
```
## PipelineExecutionStartConditionType

```python
# PipelineExecutionStartConditionType usage example

from types_aiobotocore_imagebuilder.literals import PipelineExecutionStartConditionType

def get_value() -> PipelineExecutionStartConditionType:
    return "EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE"
```

```python
# PipelineExecutionStartConditionType definition

PipelineExecutionStartConditionType = Literal[
    "EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE",
    "EXPRESSION_MATCH_ONLY",
]
```
## PipelineStatusType

```python
# PipelineStatusType usage example

from types_aiobotocore_imagebuilder.literals import PipelineStatusType

def get_value() -> PipelineStatusType:
    return "DISABLED"
```

```python
# PipelineStatusType definition

PipelineStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PlatformType

```python
# PlatformType usage example

from types_aiobotocore_imagebuilder.literals import PlatformType

def get_value() -> PlatformType:
    return "Linux"
```

```python
# PlatformType definition

PlatformType = Literal[
    "Linux",
    "Windows",
]
```
## WorkflowExecutionStatusType

```python
# WorkflowExecutionStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowExecutionStatusType

def get_value() -> WorkflowExecutionStatusType:
    return "COMPLETED"
```

```python
# WorkflowExecutionStatusType definition

WorkflowExecutionStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "PENDING",
    "ROLLBACK_COMPLETED",
    "ROLLBACK_IN_PROGRESS",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowStepExecutionRollbackStatusType

```python
# WorkflowStepExecutionRollbackStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStepExecutionRollbackStatusType

def get_value() -> WorkflowStepExecutionRollbackStatusType:
    return "COMPLETED"
```

```python
# WorkflowStepExecutionRollbackStatusType definition

WorkflowStepExecutionRollbackStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowStepExecutionStatusType

```python
# WorkflowStepExecutionStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStepExecutionStatusType

def get_value() -> WorkflowStepExecutionStatusType:
    return "COMPLETED"
```

```python
# WorkflowStepExecutionStatusType definition

WorkflowStepExecutionStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "PENDING",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowTypeType

```python
# WorkflowTypeType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowTypeType

def get_value() -> WorkflowTypeType:
    return "BUILD"
```

```python
# WorkflowTypeType definition

WorkflowTypeType = Literal[
    "BUILD",
    "DISTRIBUTION",
    "TEST",
]
```
## imagebuilderServiceName

```python
# imagebuilderServiceName usage example

from types_aiobotocore_imagebuilder.literals import imagebuilderServiceName

def get_value() -> imagebuilderServiceName:
    return "imagebuilder"
```

```python
# imagebuilderServiceName definition

imagebuilderServiceName = Literal[
    "imagebuilder",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_imagebuilder.literals import ServiceName

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

from types_aiobotocore_imagebuilder.literals import ResourceServiceName

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
