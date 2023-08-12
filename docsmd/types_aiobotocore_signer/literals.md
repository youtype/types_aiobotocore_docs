# Literals

> [Index](../README.md) > [signer](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## CategoryType

```python
# CategoryType usage example

from types_aiobotocore_signer.literals import CategoryType

def get_value() -> CategoryType:
    return "AWSIoT"
```

```python
# CategoryType definition

CategoryType = Literal[
    "AWSIoT",
]
```
## EncryptionAlgorithmType

```python
# EncryptionAlgorithmType usage example

from types_aiobotocore_signer.literals import EncryptionAlgorithmType

def get_value() -> EncryptionAlgorithmType:
    return "ECDSA"
```

```python
# EncryptionAlgorithmType definition

EncryptionAlgorithmType = Literal[
    "ECDSA",
    "RSA",
]
```
## HashAlgorithmType

```python
# HashAlgorithmType usage example

from types_aiobotocore_signer.literals import HashAlgorithmType

def get_value() -> HashAlgorithmType:
    return "SHA1"
```

```python
# HashAlgorithmType definition

HashAlgorithmType = Literal[
    "SHA1",
    "SHA256",
]
```
## ImageFormatType

```python
# ImageFormatType usage example

from types_aiobotocore_signer.literals import ImageFormatType

def get_value() -> ImageFormatType:
    return "JSON"
```

```python
# ImageFormatType definition

ImageFormatType = Literal[
    "JSON",
    "JSONDetached",
    "JSONEmbedded",
]
```
## ListSigningJobsPaginatorName

```python
# ListSigningJobsPaginatorName usage example

from types_aiobotocore_signer.literals import ListSigningJobsPaginatorName

def get_value() -> ListSigningJobsPaginatorName:
    return "list_signing_jobs"
```

```python
# ListSigningJobsPaginatorName definition

ListSigningJobsPaginatorName = Literal[
    "list_signing_jobs",
]
```
## ListSigningPlatformsPaginatorName

```python
# ListSigningPlatformsPaginatorName usage example

from types_aiobotocore_signer.literals import ListSigningPlatformsPaginatorName

def get_value() -> ListSigningPlatformsPaginatorName:
    return "list_signing_platforms"
```

```python
# ListSigningPlatformsPaginatorName definition

ListSigningPlatformsPaginatorName = Literal[
    "list_signing_platforms",
]
```
## ListSigningProfilesPaginatorName

```python
# ListSigningProfilesPaginatorName usage example

from types_aiobotocore_signer.literals import ListSigningProfilesPaginatorName

def get_value() -> ListSigningProfilesPaginatorName:
    return "list_signing_profiles"
```

```python
# ListSigningProfilesPaginatorName definition

ListSigningProfilesPaginatorName = Literal[
    "list_signing_profiles",
]
```
## SigningProfileStatusType

```python
# SigningProfileStatusType usage example

from types_aiobotocore_signer.literals import SigningProfileStatusType

def get_value() -> SigningProfileStatusType:
    return "Active"
```

```python
# SigningProfileStatusType definition

SigningProfileStatusType = Literal[
    "Active",
    "Canceled",
    "Revoked",
]
```
## SigningStatusType

```python
# SigningStatusType usage example

from types_aiobotocore_signer.literals import SigningStatusType

def get_value() -> SigningStatusType:
    return "Failed"
```

```python
# SigningStatusType definition

SigningStatusType = Literal[
    "Failed",
    "InProgress",
    "Succeeded",
]
```
## SuccessfulSigningJobWaiterName

```python
# SuccessfulSigningJobWaiterName usage example

from types_aiobotocore_signer.literals import SuccessfulSigningJobWaiterName

def get_value() -> SuccessfulSigningJobWaiterName:
    return "successful_signing_job"
```

```python
# SuccessfulSigningJobWaiterName definition

SuccessfulSigningJobWaiterName = Literal[
    "successful_signing_job",
]
```
## ValidityTypeType

```python
# ValidityTypeType usage example

from types_aiobotocore_signer.literals import ValidityTypeType

def get_value() -> ValidityTypeType:
    return "DAYS"
```

```python
# ValidityTypeType definition

ValidityTypeType = Literal[
    "DAYS",
    "MONTHS",
    "YEARS",
]
```
## signerServiceName

```python
# signerServiceName usage example

from types_aiobotocore_signer.literals import signerServiceName

def get_value() -> signerServiceName:
    return "signer"
```

```python
# signerServiceName definition

signerServiceName = Literal[
    "signer",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_signer.literals import ServiceName

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

from types_aiobotocore_signer.literals import ResourceServiceName

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

from types_aiobotocore_signer.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_signing_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_signing_jobs",
    "list_signing_platforms",
    "list_signing_profiles",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_signer.literals import WaiterName

def get_value() -> WaiterName:
    return "successful_signing_job"
```

```python
# WaiterName definition

WaiterName = Literal[
    "successful_signing_job",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_signer.literals import RegionName

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
