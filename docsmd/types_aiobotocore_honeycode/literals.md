# Literals

> [Index](../README.md) > [Honeycode](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

## ErrorCodeType

```python
# ErrorCodeType usage example

from types_aiobotocore_honeycode.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "ACCESS_DENIED"
```

```python
# ErrorCodeType definition

ErrorCodeType = Literal[
    "ACCESS_DENIED",
    "FILE_EMPTY_ERROR",
    "FILE_NOT_FOUND_ERROR",
    "FILE_PARSING_ERROR",
    "FILE_SIZE_LIMIT_ERROR",
    "INVALID_FILE_TYPE_ERROR",
    "INVALID_IMPORT_OPTIONS_ERROR",
    "INVALID_TABLE_COLUMN_ID_ERROR",
    "INVALID_TABLE_ID_ERROR",
    "INVALID_URL_ERROR",
    "RESOURCE_NOT_FOUND_ERROR",
    "SYSTEM_LIMIT_ERROR",
    "TABLE_NOT_FOUND_ERROR",
    "UNKNOWN_ERROR",
]
```
## FormatType

```python
# FormatType usage example

from types_aiobotocore_honeycode.literals import FormatType

def get_value() -> FormatType:
    return "ACCOUNTING"
```

```python
# FormatType definition

FormatType = Literal[
    "ACCOUNTING",
    "AUTO",
    "CONTACT",
    "CURRENCY",
    "DATE",
    "DATE_TIME",
    "NUMBER",
    "PERCENTAGE",
    "ROWLINK",
    "ROWSET",
    "TEXT",
    "TIME",
]
```
## ImportDataCharacterEncodingType

```python
# ImportDataCharacterEncodingType usage example

from types_aiobotocore_honeycode.literals import ImportDataCharacterEncodingType

def get_value() -> ImportDataCharacterEncodingType:
    return "ISO-8859-1"
```

```python
# ImportDataCharacterEncodingType definition

ImportDataCharacterEncodingType = Literal[
    "ISO-8859-1",
    "US-ASCII",
    "UTF-16",
    "UTF-16BE",
    "UTF-16LE",
    "UTF-8",
]
```
## ImportSourceDataFormatType

```python
# ImportSourceDataFormatType usage example

from types_aiobotocore_honeycode.literals import ImportSourceDataFormatType

def get_value() -> ImportSourceDataFormatType:
    return "DELIMITED_TEXT"
```

```python
# ImportSourceDataFormatType definition

ImportSourceDataFormatType = Literal[
    "DELIMITED_TEXT",
]
```
## ListTableColumnsPaginatorName

```python
# ListTableColumnsPaginatorName usage example

from types_aiobotocore_honeycode.literals import ListTableColumnsPaginatorName

def get_value() -> ListTableColumnsPaginatorName:
    return "list_table_columns"
```

```python
# ListTableColumnsPaginatorName definition

ListTableColumnsPaginatorName = Literal[
    "list_table_columns",
]
```
## ListTableRowsPaginatorName

```python
# ListTableRowsPaginatorName usage example

from types_aiobotocore_honeycode.literals import ListTableRowsPaginatorName

def get_value() -> ListTableRowsPaginatorName:
    return "list_table_rows"
```

```python
# ListTableRowsPaginatorName definition

ListTableRowsPaginatorName = Literal[
    "list_table_rows",
]
```
## ListTablesPaginatorName

```python
# ListTablesPaginatorName usage example

from types_aiobotocore_honeycode.literals import ListTablesPaginatorName

def get_value() -> ListTablesPaginatorName:
    return "list_tables"
```

```python
# ListTablesPaginatorName definition

ListTablesPaginatorName = Literal[
    "list_tables",
]
```
## QueryTableRowsPaginatorName

```python
# QueryTableRowsPaginatorName usage example

from types_aiobotocore_honeycode.literals import QueryTableRowsPaginatorName

def get_value() -> QueryTableRowsPaginatorName:
    return "query_table_rows"
```

```python
# QueryTableRowsPaginatorName definition

QueryTableRowsPaginatorName = Literal[
    "query_table_rows",
]
```
## TableDataImportJobStatusType

```python
# TableDataImportJobStatusType usage example

from types_aiobotocore_honeycode.literals import TableDataImportJobStatusType

def get_value() -> TableDataImportJobStatusType:
    return "COMPLETED"
```

```python
# TableDataImportJobStatusType definition

TableDataImportJobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "SUBMITTED",
]
```
## UpsertActionType

```python
# UpsertActionType usage example

from types_aiobotocore_honeycode.literals import UpsertActionType

def get_value() -> UpsertActionType:
    return "APPENDED"
```

```python
# UpsertActionType definition

UpsertActionType = Literal[
    "APPENDED",
    "UPDATED",
]
```
## HoneycodeServiceName

```python
# HoneycodeServiceName usage example

from types_aiobotocore_honeycode.literals import HoneycodeServiceName

def get_value() -> HoneycodeServiceName:
    return "honeycode"
```

```python
# HoneycodeServiceName definition

HoneycodeServiceName = Literal[
    "honeycode",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_honeycode.literals import ServiceName

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

from types_aiobotocore_honeycode.literals import ResourceServiceName

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

from types_aiobotocore_honeycode.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_table_columns"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_table_columns",
    "list_table_rows",
    "list_tables",
    "query_table_rows",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_honeycode.literals import RegionName

def get_value() -> RegionName:
    return "us-west-2"
```

```python
# RegionName definition

RegionName = Literal[
    "us-west-2",
]
```
