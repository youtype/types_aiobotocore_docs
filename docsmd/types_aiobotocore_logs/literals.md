# Literals

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#cloudwatchlogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## AnomalyDetectorStatusType

```python
# AnomalyDetectorStatusType usage example
from types_aiobotocore_logs.literals import AnomalyDetectorStatusType

def get_value() -> AnomalyDetectorStatusType:
    return "ANALYZING"
```

```python
# AnomalyDetectorStatusType definition
AnomalyDetectorStatusType = Literal[
    "ANALYZING",
    "DELETED",
    "FAILED",
    "INITIALIZING",
    "PAUSED",
    "TRAINING",
]
```
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
## DeliveryDestinationTypeType

```python
# DeliveryDestinationTypeType usage example
from types_aiobotocore_logs.literals import DeliveryDestinationTypeType

def get_value() -> DeliveryDestinationTypeType:
    return "CWL"
```

```python
# DeliveryDestinationTypeType definition
DeliveryDestinationTypeType = Literal[
    "CWL",
    "FH",
    "S3",
]
```
## DescribeConfigurationTemplatesPaginatorName

```python
# DescribeConfigurationTemplatesPaginatorName usage example
from types_aiobotocore_logs.literals import DescribeConfigurationTemplatesPaginatorName

def get_value() -> DescribeConfigurationTemplatesPaginatorName:
    return "describe_configuration_templates"
```

```python
# DescribeConfigurationTemplatesPaginatorName definition
DescribeConfigurationTemplatesPaginatorName = Literal[
    "describe_configuration_templates",
]
```
## DescribeDeliveriesPaginatorName

```python
# DescribeDeliveriesPaginatorName usage example
from types_aiobotocore_logs.literals import DescribeDeliveriesPaginatorName

def get_value() -> DescribeDeliveriesPaginatorName:
    return "describe_deliveries"
```

```python
# DescribeDeliveriesPaginatorName definition
DescribeDeliveriesPaginatorName = Literal[
    "describe_deliveries",
]
```
## DescribeDeliveryDestinationsPaginatorName

```python
# DescribeDeliveryDestinationsPaginatorName usage example
from types_aiobotocore_logs.literals import DescribeDeliveryDestinationsPaginatorName

def get_value() -> DescribeDeliveryDestinationsPaginatorName:
    return "describe_delivery_destinations"
```

```python
# DescribeDeliveryDestinationsPaginatorName definition
DescribeDeliveryDestinationsPaginatorName = Literal[
    "describe_delivery_destinations",
]
```
## DescribeDeliverySourcesPaginatorName

```python
# DescribeDeliverySourcesPaginatorName usage example
from types_aiobotocore_logs.literals import DescribeDeliverySourcesPaginatorName

def get_value() -> DescribeDeliverySourcesPaginatorName:
    return "describe_delivery_sources"
```

```python
# DescribeDeliverySourcesPaginatorName definition
DescribeDeliverySourcesPaginatorName = Literal[
    "describe_delivery_sources",
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
## EntityRejectionErrorTypeType

```python
# EntityRejectionErrorTypeType usage example
from types_aiobotocore_logs.literals import EntityRejectionErrorTypeType

def get_value() -> EntityRejectionErrorTypeType:
    return "EntitySizeTooLarge"
```

```python
# EntityRejectionErrorTypeType definition
EntityRejectionErrorTypeType = Literal[
    "EntitySizeTooLarge",
    "InvalidAttributes",
    "InvalidEntity",
    "InvalidKeyAttributes",
    "InvalidTypeValue",
    "MissingRequiredFields",
    "UnsupportedLogGroupType",
]
```
## EvaluationFrequencyType

```python
# EvaluationFrequencyType usage example
from types_aiobotocore_logs.literals import EvaluationFrequencyType

def get_value() -> EvaluationFrequencyType:
    return "FIFTEEN_MIN"
```

```python
# EvaluationFrequencyType definition
EvaluationFrequencyType = Literal[
    "FIFTEEN_MIN",
    "FIVE_MIN",
    "ONE_HOUR",
    "ONE_MIN",
    "TEN_MIN",
    "THIRTY_MIN",
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
## FlattenedElementType

```python
# FlattenedElementType usage example
from types_aiobotocore_logs.literals import FlattenedElementType

def get_value() -> FlattenedElementType:
    return "first"
```

```python
# FlattenedElementType definition
FlattenedElementType = Literal[
    "first",
    "last",
]
```
## IndexSourceType

```python
# IndexSourceType usage example
from types_aiobotocore_logs.literals import IndexSourceType

def get_value() -> IndexSourceType:
    return "ACCOUNT"
```

```python
# IndexSourceType definition
IndexSourceType = Literal[
    "ACCOUNT",
    "LOG_GROUP",
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
## IntegrationStatusType

```python
# IntegrationStatusType usage example
from types_aiobotocore_logs.literals import IntegrationStatusType

def get_value() -> IntegrationStatusType:
    return "ACTIVE"
```

```python
# IntegrationStatusType definition
IntegrationStatusType = Literal[
    "ACTIVE",
    "FAILED",
    "PROVISIONING",
]
```
## IntegrationTypeType

```python
# IntegrationTypeType usage example
from types_aiobotocore_logs.literals import IntegrationTypeType

def get_value() -> IntegrationTypeType:
    return "OPENSEARCH"
```

```python
# IntegrationTypeType definition
IntegrationTypeType = Literal[
    "OPENSEARCH",
]
```
## ListAnomaliesPaginatorName

```python
# ListAnomaliesPaginatorName usage example
from types_aiobotocore_logs.literals import ListAnomaliesPaginatorName

def get_value() -> ListAnomaliesPaginatorName:
    return "list_anomalies"
```

```python
# ListAnomaliesPaginatorName definition
ListAnomaliesPaginatorName = Literal[
    "list_anomalies",
]
```
## ListLogAnomalyDetectorsPaginatorName

```python
# ListLogAnomalyDetectorsPaginatorName usage example
from types_aiobotocore_logs.literals import ListLogAnomalyDetectorsPaginatorName

def get_value() -> ListLogAnomalyDetectorsPaginatorName:
    return "list_log_anomaly_detectors"
```

```python
# ListLogAnomalyDetectorsPaginatorName definition
ListLogAnomalyDetectorsPaginatorName = Literal[
    "list_log_anomaly_detectors",
]
```
## ListLogGroupsForQueryPaginatorName

```python
# ListLogGroupsForQueryPaginatorName usage example
from types_aiobotocore_logs.literals import ListLogGroupsForQueryPaginatorName

def get_value() -> ListLogGroupsForQueryPaginatorName:
    return "list_log_groups_for_query"
```

```python
# ListLogGroupsForQueryPaginatorName definition
ListLogGroupsForQueryPaginatorName = Literal[
    "list_log_groups_for_query",
]
```
## LogGroupClassType

```python
# LogGroupClassType usage example
from types_aiobotocore_logs.literals import LogGroupClassType

def get_value() -> LogGroupClassType:
    return "INFREQUENT_ACCESS"
```

```python
# LogGroupClassType definition
LogGroupClassType = Literal[
    "INFREQUENT_ACCESS",
    "STANDARD",
]
```
## OpenSearchResourceStatusTypeType

```python
# OpenSearchResourceStatusTypeType usage example
from types_aiobotocore_logs.literals import OpenSearchResourceStatusTypeType

def get_value() -> OpenSearchResourceStatusTypeType:
    return "ACTIVE"
```

```python
# OpenSearchResourceStatusTypeType definition
OpenSearchResourceStatusTypeType = Literal[
    "ACTIVE",
    "ERROR",
    "NOT_FOUND",
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
## OutputFormatType

```python
# OutputFormatType usage example
from types_aiobotocore_logs.literals import OutputFormatType

def get_value() -> OutputFormatType:
    return "json"
```

```python
# OutputFormatType definition
OutputFormatType = Literal[
    "json",
    "parquet",
    "plain",
    "raw",
    "w3c",
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
    "FIELD_INDEX_POLICY",
    "SUBSCRIPTION_FILTER_POLICY",
    "TRANSFORMER_POLICY",
]
```
## QueryLanguageType

```python
# QueryLanguageType usage example
from types_aiobotocore_logs.literals import QueryLanguageType

def get_value() -> QueryLanguageType:
    return "CWLI"
```

```python
# QueryLanguageType definition
QueryLanguageType = Literal[
    "CWLI",
    "PPL",
    "SQL",
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
## StateType

```python
# StateType usage example
from types_aiobotocore_logs.literals import StateType

def get_value() -> StateType:
    return "Active"
```

```python
# StateType definition
StateType = Literal[
    "Active",
    "Baseline",
    "Suppressed",
]
```
## SuppressionStateType

```python
# SuppressionStateType usage example
from types_aiobotocore_logs.literals import SuppressionStateType

def get_value() -> SuppressionStateType:
    return "SUPPRESSED"
```

```python
# SuppressionStateType definition
SuppressionStateType = Literal[
    "SUPPRESSED",
    "UNSUPPRESSED",
]
```
## SuppressionTypeType

```python
# SuppressionTypeType usage example
from types_aiobotocore_logs.literals import SuppressionTypeType

def get_value() -> SuppressionTypeType:
    return "INFINITE"
```

```python
# SuppressionTypeType definition
SuppressionTypeType = Literal[
    "INFINITE",
    "LIMITED",
]
```
## SuppressionUnitType

```python
# SuppressionUnitType usage example
from types_aiobotocore_logs.literals import SuppressionUnitType

def get_value() -> SuppressionUnitType:
    return "HOURS"
```

```python
# SuppressionUnitType definition
SuppressionUnitType = Literal[
    "HOURS",
    "MINUTES",
    "SECONDS",
]
```
## TypeType

```python
# TypeType usage example
from types_aiobotocore_logs.literals import TypeType

def get_value() -> TypeType:
    return "boolean"
```

```python
# TypeType definition
TypeType = Literal[
    "boolean",
    "double",
    "integer",
    "string",
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
    return "describe_configuration_templates"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_configuration_templates",
    "describe_deliveries",
    "describe_delivery_destinations",
    "describe_delivery_sources",
    "describe_destinations",
    "describe_export_tasks",
    "describe_log_groups",
    "describe_log_streams",
    "describe_metric_filters",
    "describe_queries",
    "describe_resource_policies",
    "describe_subscription_filters",
    "filter_log_events",
    "list_anomalies",
    "list_log_anomaly_detectors",
    "list_log_groups_for_query",
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
    "ap-southeast-5",
    "ap-southeast-7",
    "ca-central-1",
    "ca-west-1",
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
    "mx-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
