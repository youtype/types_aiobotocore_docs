# Literals

> [Index](../README.md) > [DataExchange](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## AssetTypeType

```python
# AssetTypeType usage example

from types_aiobotocore_dataexchange.literals import AssetTypeType

def get_value() -> AssetTypeType:
    return "API_GATEWAY_API"
```

```python
# AssetTypeType definition

AssetTypeType = Literal[
    "API_GATEWAY_API",
    "LAKE_FORMATION_DATA_PERMISSION",
    "REDSHIFT_DATA_SHARE",
    "S3_DATA_ACCESS",
    "S3_SNAPSHOT",
]
```
## CodeType

```python
# CodeType usage example

from types_aiobotocore_dataexchange.literals import CodeType

def get_value() -> CodeType:
    return "ACCESS_DENIED_EXCEPTION"
```

```python
# CodeType definition

CodeType = Literal[
    "ACCESS_DENIED_EXCEPTION",
    "INTERNAL_SERVER_EXCEPTION",
    "MALWARE_DETECTED",
    "MALWARE_SCAN_ENCRYPTED_FILE",
    "RESOURCE_NOT_FOUND_EXCEPTION",
    "SERVICE_QUOTA_EXCEEDED_EXCEPTION",
    "VALIDATION_EXCEPTION",
]
```
## DatabaseLFTagPolicyPermissionType

```python
# DatabaseLFTagPolicyPermissionType usage example

from types_aiobotocore_dataexchange.literals import DatabaseLFTagPolicyPermissionType

def get_value() -> DatabaseLFTagPolicyPermissionType:
    return "DESCRIBE"
```

```python
# DatabaseLFTagPolicyPermissionType definition

DatabaseLFTagPolicyPermissionType = Literal[
    "DESCRIBE",
]
```
## JobErrorLimitNameType

```python
# JobErrorLimitNameType usage example

from types_aiobotocore_dataexchange.literals import JobErrorLimitNameType

def get_value() -> JobErrorLimitNameType:
    return "AWS Lake Formation data permission assets per revision"
```

```python
# JobErrorLimitNameType definition

JobErrorLimitNameType = Literal[
    "Amazon Redshift datashare assets per revision",
    "Amazon S3 data access assets per revision",
    "Asset size in GB",
    "Assets per revision",
    "AWS Lake Formation data permission assets per revision",
]
```
## JobErrorResourceTypesType

```python
# JobErrorResourceTypesType usage example

from types_aiobotocore_dataexchange.literals import JobErrorResourceTypesType

def get_value() -> JobErrorResourceTypesType:
    return "ASSET"
```

```python
# JobErrorResourceTypesType definition

JobErrorResourceTypesType = Literal[
    "ASSET",
    "DATA_SET",
    "REVISION",
]
```
## LFPermissionType

```python
# LFPermissionType usage example

from types_aiobotocore_dataexchange.literals import LFPermissionType

def get_value() -> LFPermissionType:
    return "DESCRIBE"
```

```python
# LFPermissionType definition

LFPermissionType = Literal[
    "DESCRIBE",
    "SELECT",
]
```
## LFResourceTypeType

```python
# LFResourceTypeType usage example

from types_aiobotocore_dataexchange.literals import LFResourceTypeType

def get_value() -> LFResourceTypeType:
    return "DATABASE"
```

```python
# LFResourceTypeType definition

LFResourceTypeType = Literal[
    "DATABASE",
    "TABLE",
]
```
## LakeFormationDataPermissionTypeType

```python
# LakeFormationDataPermissionTypeType usage example

from types_aiobotocore_dataexchange.literals import LakeFormationDataPermissionTypeType

def get_value() -> LakeFormationDataPermissionTypeType:
    return "LFTagPolicy"
```

```python
# LakeFormationDataPermissionTypeType definition

LakeFormationDataPermissionTypeType = Literal[
    "LFTagPolicy",
]
```
## ListDataSetRevisionsPaginatorName

```python
# ListDataSetRevisionsPaginatorName usage example

from types_aiobotocore_dataexchange.literals import ListDataSetRevisionsPaginatorName

def get_value() -> ListDataSetRevisionsPaginatorName:
    return "list_data_set_revisions"
```

```python
# ListDataSetRevisionsPaginatorName definition

ListDataSetRevisionsPaginatorName = Literal[
    "list_data_set_revisions",
]
```
## ListDataSetsPaginatorName

```python
# ListDataSetsPaginatorName usage example

from types_aiobotocore_dataexchange.literals import ListDataSetsPaginatorName

def get_value() -> ListDataSetsPaginatorName:
    return "list_data_sets"
```

```python
# ListDataSetsPaginatorName definition

ListDataSetsPaginatorName = Literal[
    "list_data_sets",
]
```
## ListEventActionsPaginatorName

```python
# ListEventActionsPaginatorName usage example

from types_aiobotocore_dataexchange.literals import ListEventActionsPaginatorName

def get_value() -> ListEventActionsPaginatorName:
    return "list_event_actions"
```

```python
# ListEventActionsPaginatorName definition

ListEventActionsPaginatorName = Literal[
    "list_event_actions",
]
```
## ListJobsPaginatorName

```python
# ListJobsPaginatorName usage example

from types_aiobotocore_dataexchange.literals import ListJobsPaginatorName

def get_value() -> ListJobsPaginatorName:
    return "list_jobs"
```

```python
# ListJobsPaginatorName definition

ListJobsPaginatorName = Literal[
    "list_jobs",
]
```
## ListRevisionAssetsPaginatorName

```python
# ListRevisionAssetsPaginatorName usage example

from types_aiobotocore_dataexchange.literals import ListRevisionAssetsPaginatorName

def get_value() -> ListRevisionAssetsPaginatorName:
    return "list_revision_assets"
```

```python
# ListRevisionAssetsPaginatorName definition

ListRevisionAssetsPaginatorName = Literal[
    "list_revision_assets",
]
```
## OriginType

```python
# OriginType usage example

from types_aiobotocore_dataexchange.literals import OriginType

def get_value() -> OriginType:
    return "ENTITLED"
```

```python
# OriginType definition

OriginType = Literal[
    "ENTITLED",
    "OWNED",
]
```
## ProtocolTypeType

```python
# ProtocolTypeType usage example

from types_aiobotocore_dataexchange.literals import ProtocolTypeType

def get_value() -> ProtocolTypeType:
    return "REST"
```

```python
# ProtocolTypeType definition

ProtocolTypeType = Literal[
    "REST",
]
```
## ServerSideEncryptionTypesType

```python
# ServerSideEncryptionTypesType usage example

from types_aiobotocore_dataexchange.literals import ServerSideEncryptionTypesType

def get_value() -> ServerSideEncryptionTypesType:
    return "AES256"
```

```python
# ServerSideEncryptionTypesType definition

ServerSideEncryptionTypesType = Literal[
    "AES256",
    "aws:kms",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_dataexchange.literals import StateType

def get_value() -> StateType:
    return "CANCELLED"
```

```python
# StateType definition

StateType = Literal[
    "CANCELLED",
    "COMPLETED",
    "ERROR",
    "IN_PROGRESS",
    "TIMED_OUT",
    "WAITING",
]
```
## TableTagPolicyLFPermissionType

```python
# TableTagPolicyLFPermissionType usage example

from types_aiobotocore_dataexchange.literals import TableTagPolicyLFPermissionType

def get_value() -> TableTagPolicyLFPermissionType:
    return "DESCRIBE"
```

```python
# TableTagPolicyLFPermissionType definition

TableTagPolicyLFPermissionType = Literal[
    "DESCRIBE",
    "SELECT",
]
```
## TypeType

```python
# TypeType usage example

from types_aiobotocore_dataexchange.literals import TypeType

def get_value() -> TypeType:
    return "CREATE_S3_DATA_ACCESS_FROM_S3_BUCKET"
```

```python
# TypeType definition

TypeType = Literal[
    "CREATE_S3_DATA_ACCESS_FROM_S3_BUCKET",
    "EXPORT_ASSET_TO_SIGNED_URL",
    "EXPORT_ASSETS_TO_S3",
    "EXPORT_REVISIONS_TO_S3",
    "IMPORT_ASSET_FROM_API_GATEWAY_API",
    "IMPORT_ASSET_FROM_SIGNED_URL",
    "IMPORT_ASSETS_FROM_LAKE_FORMATION_TAG_POLICY",
    "IMPORT_ASSETS_FROM_REDSHIFT_DATA_SHARES",
    "IMPORT_ASSETS_FROM_S3",
]
```
## DataExchangeServiceName

```python
# DataExchangeServiceName usage example

from types_aiobotocore_dataexchange.literals import DataExchangeServiceName

def get_value() -> DataExchangeServiceName:
    return "dataexchange"
```

```python
# DataExchangeServiceName definition

DataExchangeServiceName = Literal[
    "dataexchange",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_dataexchange.literals import ServiceName

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

from types_aiobotocore_dataexchange.literals import ResourceServiceName

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

from types_aiobotocore_dataexchange.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_data_set_revisions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_data_set_revisions",
    "list_data_sets",
    "list_event_actions",
    "list_jobs",
    "list_revision_assets",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_dataexchange.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
