# Literals

> [Index](../README.md) > [LookoutMetrics](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#lookoutmetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## AggregationFunctionType

```python
# AggregationFunctionType usage example
from types_aiobotocore_lookoutmetrics.literals import AggregationFunctionType

def get_value() -> AggregationFunctionType:
    return "AVG"
```

```python
# AggregationFunctionType definition
AggregationFunctionType = Literal[
    "AVG",
    "SUM",
]
```
## AlertStatusType

```python
# AlertStatusType usage example
from types_aiobotocore_lookoutmetrics.literals import AlertStatusType

def get_value() -> AlertStatusType:
    return "ACTIVE"
```

```python
# AlertStatusType definition
AlertStatusType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## AlertTypeType

```python
# AlertTypeType usage example
from types_aiobotocore_lookoutmetrics.literals import AlertTypeType

def get_value() -> AlertTypeType:
    return "LAMBDA"
```

```python
# AlertTypeType definition
AlertTypeType = Literal[
    "LAMBDA",
    "SNS",
]
```
## AnomalyDetectionTaskStatusType

```python
# AnomalyDetectionTaskStatusType usage example
from types_aiobotocore_lookoutmetrics.literals import AnomalyDetectionTaskStatusType

def get_value() -> AnomalyDetectionTaskStatusType:
    return "COMPLETED"
```

```python
# AnomalyDetectionTaskStatusType definition
AnomalyDetectionTaskStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "FAILED_TO_SCHEDULE",
    "IN_PROGRESS",
    "PENDING",
]
```
## AnomalyDetectorFailureTypeType

```python
# AnomalyDetectorFailureTypeType usage example
from types_aiobotocore_lookoutmetrics.literals import AnomalyDetectorFailureTypeType

def get_value() -> AnomalyDetectorFailureTypeType:
    return "ACTIVATION_FAILURE"
```

```python
# AnomalyDetectorFailureTypeType definition
AnomalyDetectorFailureTypeType = Literal[
    "ACTIVATION_FAILURE",
    "BACK_TEST_ACTIVATION_FAILURE",
    "DEACTIVATION_FAILURE",
    "DELETION_FAILURE",
]
```
## AnomalyDetectorStatusType

```python
# AnomalyDetectorStatusType usage example
from types_aiobotocore_lookoutmetrics.literals import AnomalyDetectorStatusType

def get_value() -> AnomalyDetectorStatusType:
    return "ACTIVATING"
```

```python
# AnomalyDetectorStatusType definition
AnomalyDetectorStatusType = Literal[
    "ACTIVATING",
    "ACTIVE",
    "BACK_TEST_ACTIVATING",
    "BACK_TEST_ACTIVE",
    "BACK_TEST_COMPLETE",
    "DEACTIVATED",
    "DEACTIVATING",
    "DELETING",
    "FAILED",
    "INACTIVE",
    "LEARNING",
]
```
## CSVFileCompressionType

```python
# CSVFileCompressionType usage example
from types_aiobotocore_lookoutmetrics.literals import CSVFileCompressionType

def get_value() -> CSVFileCompressionType:
    return "GZIP"
```

```python
# CSVFileCompressionType definition
CSVFileCompressionType = Literal[
    "GZIP",
    "NONE",
]
```
## ConfidenceType

```python
# ConfidenceType usage example
from types_aiobotocore_lookoutmetrics.literals import ConfidenceType

def get_value() -> ConfidenceType:
    return "HIGH"
```

```python
# ConfidenceType definition
ConfidenceType = Literal[
    "HIGH",
    "LOW",
    "NONE",
]
```
## DataQualityMetricTypeType

```python
# DataQualityMetricTypeType usage example
from types_aiobotocore_lookoutmetrics.literals import DataQualityMetricTypeType

def get_value() -> DataQualityMetricTypeType:
    return "BACKTEST_INFERENCE_DATA_END_TIME_STAMP"
```

```python
# DataQualityMetricTypeType definition
DataQualityMetricTypeType = Literal[
    "BACKTEST_INFERENCE_DATA_END_TIME_STAMP",
    "BACKTEST_INFERENCE_DATA_START_TIME_STAMP",
    "BACKTEST_TRAINING_DATA_END_TIME_STAMP",
    "BACKTEST_TRAINING_DATA_START_TIME_STAMP",
    "COLUMN_COMPLETENESS",
    "DIMENSION_UNIQUENESS",
    "INVALID_ROWS_COMPLIANCE",
    "ROWS_PARTIAL_COMPLIANCE",
    "ROWS_PROCESSED",
    "TIME_SERIES_COUNT",
]
```
## FilterOperationType

```python
# FilterOperationType usage example
from types_aiobotocore_lookoutmetrics.literals import FilterOperationType

def get_value() -> FilterOperationType:
    return "EQUALS"
```

```python
# FilterOperationType definition
FilterOperationType = Literal[
    "EQUALS",
]
```
## FrequencyType

```python
# FrequencyType usage example
from types_aiobotocore_lookoutmetrics.literals import FrequencyType

def get_value() -> FrequencyType:
    return "P1D"
```

```python
# FrequencyType definition
FrequencyType = Literal[
    "P1D",
    "PT10M",
    "PT1H",
    "PT5M",
]
```
## JsonFileCompressionType

```python
# JsonFileCompressionType usage example
from types_aiobotocore_lookoutmetrics.literals import JsonFileCompressionType

def get_value() -> JsonFileCompressionType:
    return "GZIP"
```

```python
# JsonFileCompressionType definition
JsonFileCompressionType = Literal[
    "GZIP",
    "NONE",
]
```
## RelationshipTypeType

```python
# RelationshipTypeType usage example
from types_aiobotocore_lookoutmetrics.literals import RelationshipTypeType

def get_value() -> RelationshipTypeType:
    return "CAUSE_OF_INPUT_ANOMALY_GROUP"
```

```python
# RelationshipTypeType definition
RelationshipTypeType = Literal[
    "CAUSE_OF_INPUT_ANOMALY_GROUP",
    "EFFECT_OF_INPUT_ANOMALY_GROUP",
]
```
## SnsFormatType

```python
# SnsFormatType usage example
from types_aiobotocore_lookoutmetrics.literals import SnsFormatType

def get_value() -> SnsFormatType:
    return "JSON"
```

```python
# SnsFormatType definition
SnsFormatType = Literal[
    "JSON",
    "LONG_TEXT",
    "SHORT_TEXT",
]
```
## LookoutMetricsServiceName

```python
# LookoutMetricsServiceName usage example
from types_aiobotocore_lookoutmetrics.literals import LookoutMetricsServiceName

def get_value() -> LookoutMetricsServiceName:
    return "lookoutmetrics"
```

```python
# LookoutMetricsServiceName definition
LookoutMetricsServiceName = Literal[
    "lookoutmetrics",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_lookoutmetrics.literals import ServiceName

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
    "aiops",
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
    "arc-region-switch",
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
    "bcm-dashboards",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bcm-recommended-actions",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-agentcore",
    "bedrock-agentcore-control",
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
    "evs",
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
    "gameliftstreams",
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
    "iot-managed-integrations",
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
    "keyspacesstreams",
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
    "mpa",
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
    "odb",
    "omics",
    "opensearch",
    "opensearchserverless",
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
    "s3vectors",
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
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-guiconnect",
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
    "workspaces-instances",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_lookoutmetrics.literals import ResourceServiceName

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
    "s3",
    "sns",
    "sqs",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_lookoutmetrics.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition
RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
