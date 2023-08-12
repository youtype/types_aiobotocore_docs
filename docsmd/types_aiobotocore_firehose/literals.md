# Literals

> [Index](../README.md) > [Firehose](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Firehose](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
    type annotations stubs module [types-aiobotocore-firehose](https://pypi.org/project/types-aiobotocore-firehose/).

## AmazonOpenSearchServerlessS3BackupModeType

```python
# AmazonOpenSearchServerlessS3BackupModeType usage example

from types_aiobotocore_firehose.literals import AmazonOpenSearchServerlessS3BackupModeType

def get_value() -> AmazonOpenSearchServerlessS3BackupModeType:
    return "AllDocuments"
```

```python
# AmazonOpenSearchServerlessS3BackupModeType definition

AmazonOpenSearchServerlessS3BackupModeType = Literal[
    "AllDocuments",
    "FailedDocumentsOnly",
]
```
## AmazonopensearchserviceIndexRotationPeriodType

```python
# AmazonopensearchserviceIndexRotationPeriodType usage example

from types_aiobotocore_firehose.literals import AmazonopensearchserviceIndexRotationPeriodType

def get_value() -> AmazonopensearchserviceIndexRotationPeriodType:
    return "NoRotation"
```

```python
# AmazonopensearchserviceIndexRotationPeriodType definition

AmazonopensearchserviceIndexRotationPeriodType = Literal[
    "NoRotation",
    "OneDay",
    "OneHour",
    "OneMonth",
    "OneWeek",
]
```
## AmazonopensearchserviceS3BackupModeType

```python
# AmazonopensearchserviceS3BackupModeType usage example

from types_aiobotocore_firehose.literals import AmazonopensearchserviceS3BackupModeType

def get_value() -> AmazonopensearchserviceS3BackupModeType:
    return "AllDocuments"
```

```python
# AmazonopensearchserviceS3BackupModeType definition

AmazonopensearchserviceS3BackupModeType = Literal[
    "AllDocuments",
    "FailedDocumentsOnly",
]
```
## CompressionFormatType

```python
# CompressionFormatType usage example

from types_aiobotocore_firehose.literals import CompressionFormatType

def get_value() -> CompressionFormatType:
    return "GZIP"
```

```python
# CompressionFormatType definition

CompressionFormatType = Literal[
    "GZIP",
    "HADOOP_SNAPPY",
    "Snappy",
    "UNCOMPRESSED",
    "ZIP",
]
```
## ContentEncodingType

```python
# ContentEncodingType usage example

from types_aiobotocore_firehose.literals import ContentEncodingType

def get_value() -> ContentEncodingType:
    return "GZIP"
```

```python
# ContentEncodingType definition

ContentEncodingType = Literal[
    "GZIP",
    "NONE",
]
```
## DeliveryStreamEncryptionStatusType

```python
# DeliveryStreamEncryptionStatusType usage example

from types_aiobotocore_firehose.literals import DeliveryStreamEncryptionStatusType

def get_value() -> DeliveryStreamEncryptionStatusType:
    return "DISABLED"
```

```python
# DeliveryStreamEncryptionStatusType definition

DeliveryStreamEncryptionStatusType = Literal[
    "DISABLED",
    "DISABLING",
    "DISABLING_FAILED",
    "ENABLED",
    "ENABLING",
    "ENABLING_FAILED",
]
```
## DeliveryStreamFailureTypeType

```python
# DeliveryStreamFailureTypeType usage example

from types_aiobotocore_firehose.literals import DeliveryStreamFailureTypeType

def get_value() -> DeliveryStreamFailureTypeType:
    return "CREATE_ENI_FAILED"
```

```python
# DeliveryStreamFailureTypeType definition

DeliveryStreamFailureTypeType = Literal[
    "CREATE_ENI_FAILED",
    "CREATE_KMS_GRANT_FAILED",
    "DELETE_ENI_FAILED",
    "DISABLED_KMS_KEY",
    "ENI_ACCESS_DENIED",
    "INVALID_KMS_KEY",
    "KMS_ACCESS_DENIED",
    "KMS_KEY_NOT_FOUND",
    "KMS_OPT_IN_REQUIRED",
    "RETIRE_KMS_GRANT_FAILED",
    "SECURITY_GROUP_ACCESS_DENIED",
    "SECURITY_GROUP_NOT_FOUND",
    "SUBNET_ACCESS_DENIED",
    "SUBNET_NOT_FOUND",
    "UNKNOWN_ERROR",
]
```
## DeliveryStreamStatusType

```python
# DeliveryStreamStatusType usage example

from types_aiobotocore_firehose.literals import DeliveryStreamStatusType

def get_value() -> DeliveryStreamStatusType:
    return "ACTIVE"
```

```python
# DeliveryStreamStatusType definition

DeliveryStreamStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATING_FAILED",
    "DELETING",
    "DELETING_FAILED",
]
```
## DeliveryStreamTypeType

```python
# DeliveryStreamTypeType usage example

from types_aiobotocore_firehose.literals import DeliveryStreamTypeType

def get_value() -> DeliveryStreamTypeType:
    return "DirectPut"
```

```python
# DeliveryStreamTypeType definition

DeliveryStreamTypeType = Literal[
    "DirectPut",
    "KinesisStreamAsSource",
]
```
## ElasticsearchIndexRotationPeriodType

```python
# ElasticsearchIndexRotationPeriodType usage example

from types_aiobotocore_firehose.literals import ElasticsearchIndexRotationPeriodType

def get_value() -> ElasticsearchIndexRotationPeriodType:
    return "NoRotation"
```

```python
# ElasticsearchIndexRotationPeriodType definition

ElasticsearchIndexRotationPeriodType = Literal[
    "NoRotation",
    "OneDay",
    "OneHour",
    "OneMonth",
    "OneWeek",
]
```
## ElasticsearchS3BackupModeType

```python
# ElasticsearchS3BackupModeType usage example

from types_aiobotocore_firehose.literals import ElasticsearchS3BackupModeType

def get_value() -> ElasticsearchS3BackupModeType:
    return "AllDocuments"
```

```python
# ElasticsearchS3BackupModeType definition

ElasticsearchS3BackupModeType = Literal[
    "AllDocuments",
    "FailedDocumentsOnly",
]
```
## HECEndpointTypeType

```python
# HECEndpointTypeType usage example

from types_aiobotocore_firehose.literals import HECEndpointTypeType

def get_value() -> HECEndpointTypeType:
    return "Event"
```

```python
# HECEndpointTypeType definition

HECEndpointTypeType = Literal[
    "Event",
    "Raw",
]
```
## HttpEndpointS3BackupModeType

```python
# HttpEndpointS3BackupModeType usage example

from types_aiobotocore_firehose.literals import HttpEndpointS3BackupModeType

def get_value() -> HttpEndpointS3BackupModeType:
    return "AllData"
```

```python
# HttpEndpointS3BackupModeType definition

HttpEndpointS3BackupModeType = Literal[
    "AllData",
    "FailedDataOnly",
]
```
## KeyTypeType

```python
# KeyTypeType usage example

from types_aiobotocore_firehose.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "AWS_OWNED_CMK"
```

```python
# KeyTypeType definition

KeyTypeType = Literal[
    "AWS_OWNED_CMK",
    "CUSTOMER_MANAGED_CMK",
]
```
## NoEncryptionConfigType

```python
# NoEncryptionConfigType usage example

from types_aiobotocore_firehose.literals import NoEncryptionConfigType

def get_value() -> NoEncryptionConfigType:
    return "NoEncryption"
```

```python
# NoEncryptionConfigType definition

NoEncryptionConfigType = Literal[
    "NoEncryption",
]
```
## OrcCompressionType

```python
# OrcCompressionType usage example

from types_aiobotocore_firehose.literals import OrcCompressionType

def get_value() -> OrcCompressionType:
    return "NONE"
```

```python
# OrcCompressionType definition

OrcCompressionType = Literal[
    "NONE",
    "SNAPPY",
    "ZLIB",
]
```
## OrcFormatVersionType

```python
# OrcFormatVersionType usage example

from types_aiobotocore_firehose.literals import OrcFormatVersionType

def get_value() -> OrcFormatVersionType:
    return "V0_11"
```

```python
# OrcFormatVersionType definition

OrcFormatVersionType = Literal[
    "V0_11",
    "V0_12",
]
```
## ParquetCompressionType

```python
# ParquetCompressionType usage example

from types_aiobotocore_firehose.literals import ParquetCompressionType

def get_value() -> ParquetCompressionType:
    return "GZIP"
```

```python
# ParquetCompressionType definition

ParquetCompressionType = Literal[
    "GZIP",
    "SNAPPY",
    "UNCOMPRESSED",
]
```
## ParquetWriterVersionType

```python
# ParquetWriterVersionType usage example

from types_aiobotocore_firehose.literals import ParquetWriterVersionType

def get_value() -> ParquetWriterVersionType:
    return "V1"
```

```python
# ParquetWriterVersionType definition

ParquetWriterVersionType = Literal[
    "V1",
    "V2",
]
```
## ProcessorParameterNameType

```python
# ProcessorParameterNameType usage example

from types_aiobotocore_firehose.literals import ProcessorParameterNameType

def get_value() -> ProcessorParameterNameType:
    return "BufferIntervalInSeconds"
```

```python
# ProcessorParameterNameType definition

ProcessorParameterNameType = Literal[
    "BufferIntervalInSeconds",
    "BufferSizeInMBs",
    "Delimiter",
    "JsonParsingEngine",
    "LambdaArn",
    "MetadataExtractionQuery",
    "NumberOfRetries",
    "RoleArn",
    "SubRecordType",
]
```
## ProcessorTypeType

```python
# ProcessorTypeType usage example

from types_aiobotocore_firehose.literals import ProcessorTypeType

def get_value() -> ProcessorTypeType:
    return "AppendDelimiterToRecord"
```

```python
# ProcessorTypeType definition

ProcessorTypeType = Literal[
    "AppendDelimiterToRecord",
    "Lambda",
    "MetadataExtraction",
    "RecordDeAggregation",
]
```
## RedshiftS3BackupModeType

```python
# RedshiftS3BackupModeType usage example

from types_aiobotocore_firehose.literals import RedshiftS3BackupModeType

def get_value() -> RedshiftS3BackupModeType:
    return "Disabled"
```

```python
# RedshiftS3BackupModeType definition

RedshiftS3BackupModeType = Literal[
    "Disabled",
    "Enabled",
]
```
## S3BackupModeType

```python
# S3BackupModeType usage example

from types_aiobotocore_firehose.literals import S3BackupModeType

def get_value() -> S3BackupModeType:
    return "Disabled"
```

```python
# S3BackupModeType definition

S3BackupModeType = Literal[
    "Disabled",
    "Enabled",
]
```
## SplunkS3BackupModeType

```python
# SplunkS3BackupModeType usage example

from types_aiobotocore_firehose.literals import SplunkS3BackupModeType

def get_value() -> SplunkS3BackupModeType:
    return "AllEvents"
```

```python
# SplunkS3BackupModeType definition

SplunkS3BackupModeType = Literal[
    "AllEvents",
    "FailedEventsOnly",
]
```
## FirehoseServiceName

```python
# FirehoseServiceName usage example

from types_aiobotocore_firehose.literals import FirehoseServiceName

def get_value() -> FirehoseServiceName:
    return "firehose"
```

```python
# FirehoseServiceName definition

FirehoseServiceName = Literal[
    "firehose",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_firehose.literals import ServiceName

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

from types_aiobotocore_firehose.literals import ResourceServiceName

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

from types_aiobotocore_firehose.literals import RegionName

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
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
