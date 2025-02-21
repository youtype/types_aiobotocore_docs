# Literals

> [Index](../README.md) > [LookoutforVision](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#lookoutforvision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## DatasetStatusType

```python
# DatasetStatusType usage example
from types_aiobotocore_lookoutvision.literals import DatasetStatusType

def get_value() -> DatasetStatusType:
    return "CREATE_COMPLETE"
```

```python
# DatasetStatusType definition
DatasetStatusType = Literal[
    "CREATE_COMPLETE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_COMPLETE",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "UPDATE_COMPLETE",
    "UPDATE_FAILED_ROLLBACK_COMPLETE",
    "UPDATE_FAILED_ROLLBACK_IN_PROGRESS",
    "UPDATE_IN_PROGRESS",
]
```
## ListDatasetEntriesPaginatorName

```python
# ListDatasetEntriesPaginatorName usage example
from types_aiobotocore_lookoutvision.literals import ListDatasetEntriesPaginatorName

def get_value() -> ListDatasetEntriesPaginatorName:
    return "list_dataset_entries"
```

```python
# ListDatasetEntriesPaginatorName definition
ListDatasetEntriesPaginatorName = Literal[
    "list_dataset_entries",
]
```
## ListModelPackagingJobsPaginatorName

```python
# ListModelPackagingJobsPaginatorName usage example
from types_aiobotocore_lookoutvision.literals import ListModelPackagingJobsPaginatorName

def get_value() -> ListModelPackagingJobsPaginatorName:
    return "list_model_packaging_jobs"
```

```python
# ListModelPackagingJobsPaginatorName definition
ListModelPackagingJobsPaginatorName = Literal[
    "list_model_packaging_jobs",
]
```
## ListModelsPaginatorName

```python
# ListModelsPaginatorName usage example
from types_aiobotocore_lookoutvision.literals import ListModelsPaginatorName

def get_value() -> ListModelsPaginatorName:
    return "list_models"
```

```python
# ListModelsPaginatorName definition
ListModelsPaginatorName = Literal[
    "list_models",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example
from types_aiobotocore_lookoutvision.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition
ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ModelHostingStatusType

```python
# ModelHostingStatusType usage example
from types_aiobotocore_lookoutvision.literals import ModelHostingStatusType

def get_value() -> ModelHostingStatusType:
    return "HOSTED"
```

```python
# ModelHostingStatusType definition
ModelHostingStatusType = Literal[
    "HOSTED",
    "HOSTING_FAILED",
    "STARTING_HOSTING",
    "STOPPING_HOSTING",
    "SYSTEM_UPDATING",
]
```
## ModelPackagingJobStatusType

```python
# ModelPackagingJobStatusType usage example
from types_aiobotocore_lookoutvision.literals import ModelPackagingJobStatusType

def get_value() -> ModelPackagingJobStatusType:
    return "CREATED"
```

```python
# ModelPackagingJobStatusType definition
ModelPackagingJobStatusType = Literal[
    "CREATED",
    "FAILED",
    "RUNNING",
    "SUCCEEDED",
]
```
## ModelStatusType

```python
# ModelStatusType usage example
from types_aiobotocore_lookoutvision.literals import ModelStatusType

def get_value() -> ModelStatusType:
    return "DELETING"
```

```python
# ModelStatusType definition
ModelStatusType = Literal[
    "DELETING",
    "HOSTED",
    "HOSTING_FAILED",
    "STARTING_HOSTING",
    "STOPPING_HOSTING",
    "SYSTEM_UPDATING",
    "TRAINED",
    "TRAINING",
    "TRAINING_FAILED",
]
```
## TargetDeviceType

```python
# TargetDeviceType usage example
from types_aiobotocore_lookoutvision.literals import TargetDeviceType

def get_value() -> TargetDeviceType:
    return "jetson_xavier"
```

```python
# TargetDeviceType definition
TargetDeviceType = Literal[
    "jetson_xavier",
]
```
## TargetPlatformAcceleratorType

```python
# TargetPlatformAcceleratorType usage example
from types_aiobotocore_lookoutvision.literals import TargetPlatformAcceleratorType

def get_value() -> TargetPlatformAcceleratorType:
    return "NVIDIA"
```

```python
# TargetPlatformAcceleratorType definition
TargetPlatformAcceleratorType = Literal[
    "NVIDIA",
]
```
## TargetPlatformArchType

```python
# TargetPlatformArchType usage example
from types_aiobotocore_lookoutvision.literals import TargetPlatformArchType

def get_value() -> TargetPlatformArchType:
    return "ARM64"
```

```python
# TargetPlatformArchType definition
TargetPlatformArchType = Literal[
    "ARM64",
    "X86_64",
]
```
## TargetPlatformOsType

```python
# TargetPlatformOsType usage example
from types_aiobotocore_lookoutvision.literals import TargetPlatformOsType

def get_value() -> TargetPlatformOsType:
    return "LINUX"
```

```python
# TargetPlatformOsType definition
TargetPlatformOsType = Literal[
    "LINUX",
]
```
## LookoutforVisionServiceName

```python
# LookoutforVisionServiceName usage example
from types_aiobotocore_lookoutvision.literals import LookoutforVisionServiceName

def get_value() -> LookoutforVisionServiceName:
    return "lookoutvision"
```

```python
# LookoutforVisionServiceName definition
LookoutforVisionServiceName = Literal[
    "lookoutvision",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_lookoutvision.literals import ServiceName

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
from types_aiobotocore_lookoutvision.literals import ResourceServiceName

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
from types_aiobotocore_lookoutvision.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_dataset_entries"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_dataset_entries",
    "list_model_packaging_jobs",
    "list_models",
    "list_projects",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_lookoutvision.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition
RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "eu-central-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
