# Literals

> [Index](../README.md) > [SecurityLake](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## AccessTypeType

```python
# AccessTypeType usage example

from types_aiobotocore_securitylake.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "LAKEFORMATION"
```

```python
# AccessTypeType definition

AccessTypeType = Literal[
    "LAKEFORMATION",
    "S3",
]
```
## AwsLogSourceNameType

```python
# AwsLogSourceNameType usage example

from types_aiobotocore_securitylake.literals import AwsLogSourceNameType

def get_value() -> AwsLogSourceNameType:
    return "CLOUD_TRAIL_MGMT"
```

```python
# AwsLogSourceNameType definition

AwsLogSourceNameType = Literal[
    "CLOUD_TRAIL_MGMT",
    "LAMBDA_EXECUTION",
    "ROUTE53",
    "S3_DATA",
    "SH_FINDINGS",
    "VPC_FLOW",
]
```
## DataLakeStatusType

```python
# DataLakeStatusType usage example

from types_aiobotocore_securitylake.literals import DataLakeStatusType

def get_value() -> DataLakeStatusType:
    return "COMPLETED"
```

```python
# DataLakeStatusType definition

DataLakeStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "INITIALIZED",
    "PENDING",
]
```
## GetDataLakeSourcesPaginatorName

```python
# GetDataLakeSourcesPaginatorName usage example

from types_aiobotocore_securitylake.literals import GetDataLakeSourcesPaginatorName

def get_value() -> GetDataLakeSourcesPaginatorName:
    return "get_data_lake_sources"
```

```python
# GetDataLakeSourcesPaginatorName definition

GetDataLakeSourcesPaginatorName = Literal[
    "get_data_lake_sources",
]
```
## HttpMethodType

```python
# HttpMethodType usage example

from types_aiobotocore_securitylake.literals import HttpMethodType

def get_value() -> HttpMethodType:
    return "POST"
```

```python
# HttpMethodType definition

HttpMethodType = Literal[
    "POST",
    "PUT",
]
```
## ListDataLakeExceptionsPaginatorName

```python
# ListDataLakeExceptionsPaginatorName usage example

from types_aiobotocore_securitylake.literals import ListDataLakeExceptionsPaginatorName

def get_value() -> ListDataLakeExceptionsPaginatorName:
    return "list_data_lake_exceptions"
```

```python
# ListDataLakeExceptionsPaginatorName definition

ListDataLakeExceptionsPaginatorName = Literal[
    "list_data_lake_exceptions",
]
```
## ListLogSourcesPaginatorName

```python
# ListLogSourcesPaginatorName usage example

from types_aiobotocore_securitylake.literals import ListLogSourcesPaginatorName

def get_value() -> ListLogSourcesPaginatorName:
    return "list_log_sources"
```

```python
# ListLogSourcesPaginatorName definition

ListLogSourcesPaginatorName = Literal[
    "list_log_sources",
]
```
## ListSubscribersPaginatorName

```python
# ListSubscribersPaginatorName usage example

from types_aiobotocore_securitylake.literals import ListSubscribersPaginatorName

def get_value() -> ListSubscribersPaginatorName:
    return "list_subscribers"
```

```python
# ListSubscribersPaginatorName definition

ListSubscribersPaginatorName = Literal[
    "list_subscribers",
]
```
## SourceCollectionStatusType

```python
# SourceCollectionStatusType usage example

from types_aiobotocore_securitylake.literals import SourceCollectionStatusType

def get_value() -> SourceCollectionStatusType:
    return "COLLECTING"
```

```python
# SourceCollectionStatusType definition

SourceCollectionStatusType = Literal[
    "COLLECTING",
    "MISCONFIGURED",
    "NOT_COLLECTING",
]
```
## SubscriberStatusType

```python
# SubscriberStatusType usage example

from types_aiobotocore_securitylake.literals import SubscriberStatusType

def get_value() -> SubscriberStatusType:
    return "ACTIVE"
```

```python
# SubscriberStatusType definition

SubscriberStatusType = Literal[
    "ACTIVE",
    "DEACTIVATED",
    "PENDING",
    "READY",
]
```
## SecurityLakeServiceName

```python
# SecurityLakeServiceName usage example

from types_aiobotocore_securitylake.literals import SecurityLakeServiceName

def get_value() -> SecurityLakeServiceName:
    return "securitylake"
```

```python
# SecurityLakeServiceName definition

SecurityLakeServiceName = Literal[
    "securitylake",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_securitylake.literals import ServiceName

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

from types_aiobotocore_securitylake.literals import ResourceServiceName

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

from types_aiobotocore_securitylake.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_data_lake_sources"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_data_lake_sources",
    "list_data_lake_exceptions",
    "list_log_sources",
    "list_subscribers",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_securitylake.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
