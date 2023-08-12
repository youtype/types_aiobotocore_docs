# Literals

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## DataProtectionStatusType

```python
# DataProtectionStatusType usage example

from types_aiobotocore_logs.literals import DataProtectionStatusType

def get_value() -> DataProtectionStatusType:
    return "ACTIVATED"
```

```python
# DataProtectionStatusType definition

DataProtectionStatusType = Literal[
    "ACTIVATED",
    "ARCHIVED",
    "DELETED",
    "DISABLED",
]
```
## DescribeDestinationsPaginatorName

```python
# DescribeDestinationsPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeDestinationsPaginatorName

def get_value() -> DescribeDestinationsPaginatorName:
    return "describe_destinations"
```

```python
# DescribeDestinationsPaginatorName definition

DescribeDestinationsPaginatorName = Literal[
    "describe_destinations",
]
```
## DescribeExportTasksPaginatorName

```python
# DescribeExportTasksPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeExportTasksPaginatorName

def get_value() -> DescribeExportTasksPaginatorName:
    return "describe_export_tasks"
```

```python
# DescribeExportTasksPaginatorName definition

DescribeExportTasksPaginatorName = Literal[
    "describe_export_tasks",
]
```
## DescribeLogGroupsPaginatorName

```python
# DescribeLogGroupsPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeLogGroupsPaginatorName

def get_value() -> DescribeLogGroupsPaginatorName:
    return "describe_log_groups"
```

```python
# DescribeLogGroupsPaginatorName definition

DescribeLogGroupsPaginatorName = Literal[
    "describe_log_groups",
]
```
## DescribeLogStreamsPaginatorName

```python
# DescribeLogStreamsPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeLogStreamsPaginatorName

def get_value() -> DescribeLogStreamsPaginatorName:
    return "describe_log_streams"
```

```python
# DescribeLogStreamsPaginatorName definition

DescribeLogStreamsPaginatorName = Literal[
    "describe_log_streams",
]
```
## DescribeMetricFiltersPaginatorName

```python
# DescribeMetricFiltersPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeMetricFiltersPaginatorName

def get_value() -> DescribeMetricFiltersPaginatorName:
    return "describe_metric_filters"
```

```python
# DescribeMetricFiltersPaginatorName definition

DescribeMetricFiltersPaginatorName = Literal[
    "describe_metric_filters",
]
```
## DescribeQueriesPaginatorName

```python
# DescribeQueriesPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeQueriesPaginatorName

def get_value() -> DescribeQueriesPaginatorName:
    return "describe_queries"
```

```python
# DescribeQueriesPaginatorName definition

DescribeQueriesPaginatorName = Literal[
    "describe_queries",
]
```
## DescribeResourcePoliciesPaginatorName

```python
# DescribeResourcePoliciesPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeResourcePoliciesPaginatorName

def get_value() -> DescribeResourcePoliciesPaginatorName:
    return "describe_resource_policies"
```

```python
# DescribeResourcePoliciesPaginatorName definition

DescribeResourcePoliciesPaginatorName = Literal[
    "describe_resource_policies",
]
```
## DescribeSubscriptionFiltersPaginatorName

```python
# DescribeSubscriptionFiltersPaginatorName usage example

from types_aiobotocore_logs.literals import DescribeSubscriptionFiltersPaginatorName

def get_value() -> DescribeSubscriptionFiltersPaginatorName:
    return "describe_subscription_filters"
```

```python
# DescribeSubscriptionFiltersPaginatorName definition

DescribeSubscriptionFiltersPaginatorName = Literal[
    "describe_subscription_filters",
]
```
## DistributionType

```python
# DistributionType usage example

from types_aiobotocore_logs.literals import DistributionType

def get_value() -> DistributionType:
    return "ByLogStream"
```

```python
# DistributionType definition

DistributionType = Literal[
    "ByLogStream",
    "Random",
]
```
## ExportTaskStatusCodeType

```python
# ExportTaskStatusCodeType usage example

from types_aiobotocore_logs.literals import ExportTaskStatusCodeType

def get_value() -> ExportTaskStatusCodeType:
    return "CANCELLED"
```

```python
# ExportTaskStatusCodeType definition

ExportTaskStatusCodeType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "PENDING_CANCEL",
    "RUNNING",
]
```
## FilterLogEventsPaginatorName

```python
# FilterLogEventsPaginatorName usage example

from types_aiobotocore_logs.literals import FilterLogEventsPaginatorName

def get_value() -> FilterLogEventsPaginatorName:
    return "filter_log_events"
```

```python
# FilterLogEventsPaginatorName definition

FilterLogEventsPaginatorName = Literal[
    "filter_log_events",
]
```
## InheritedPropertyType

```python
# InheritedPropertyType usage example

from types_aiobotocore_logs.literals import InheritedPropertyType

def get_value() -> InheritedPropertyType:
    return "ACCOUNT_DATA_PROTECTION"
```

```python
# InheritedPropertyType definition

InheritedPropertyType = Literal[
    "ACCOUNT_DATA_PROTECTION",
]
```
## OrderByType

```python
# OrderByType usage example

from types_aiobotocore_logs.literals import OrderByType

def get_value() -> OrderByType:
    return "LastEventTime"
```

```python
# OrderByType definition

OrderByType = Literal[
    "LastEventTime",
    "LogStreamName",
]
```
## PolicyTypeType

```python
# PolicyTypeType usage example

from types_aiobotocore_logs.literals import PolicyTypeType

def get_value() -> PolicyTypeType:
    return "DATA_PROTECTION_POLICY"
```

```python
# PolicyTypeType definition

PolicyTypeType = Literal[
    "DATA_PROTECTION_POLICY",
]
```
## QueryStatusType

```python
# QueryStatusType usage example

from types_aiobotocore_logs.literals import QueryStatusType

def get_value() -> QueryStatusType:
    return "Cancelled"
```

```python
# QueryStatusType definition

QueryStatusType = Literal[
    "Cancelled",
    "Complete",
    "Failed",
    "Running",
    "Scheduled",
    "Timeout",
    "Unknown",
]
```
## ScopeType

```python
# ScopeType usage example

from types_aiobotocore_logs.literals import ScopeType

def get_value() -> ScopeType:
    return "ALL"
```

```python
# ScopeType definition

ScopeType = Literal[
    "ALL",
]
```
## StandardUnitType

```python
# StandardUnitType usage example

from types_aiobotocore_logs.literals import StandardUnitType

def get_value() -> StandardUnitType:
    return "Bits"
```

```python
# StandardUnitType definition

StandardUnitType = Literal[
    "Bits",
    "Bits/Second",
    "Bytes",
    "Bytes/Second",
    "Count",
    "Count/Second",
    "Gigabits",
    "Gigabits/Second",
    "Gigabytes",
    "Gigabytes/Second",
    "Kilobits",
    "Kilobits/Second",
    "Kilobytes",
    "Kilobytes/Second",
    "Megabits",
    "Megabits/Second",
    "Megabytes",
    "Megabytes/Second",
    "Microseconds",
    "Milliseconds",
    "None",
    "Percent",
    "Seconds",
    "Terabits",
    "Terabits/Second",
    "Terabytes",
    "Terabytes/Second",
]
```
## CloudWatchLogsServiceName

```python
# CloudWatchLogsServiceName usage example

from types_aiobotocore_logs.literals import CloudWatchLogsServiceName

def get_value() -> CloudWatchLogsServiceName:
    return "logs"
```

```python
# CloudWatchLogsServiceName definition

CloudWatchLogsServiceName = Literal[
    "logs",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_logs.literals import ServiceName

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

from types_aiobotocore_logs.literals import ResourceServiceName

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

from types_aiobotocore_logs.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_destinations"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_destinations",
    "describe_export_tasks",
    "describe_log_groups",
    "describe_log_streams",
    "describe_metric_filters",
    "describe_queries",
    "describe_resource_policies",
    "describe_subscription_filters",
    "filter_log_events",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_logs.literals import RegionName

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
