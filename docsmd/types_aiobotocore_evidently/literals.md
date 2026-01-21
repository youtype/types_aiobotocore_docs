# Literals

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## ChangeDirectionEnumType

```python
# ChangeDirectionEnumType usage example
from types_aiobotocore_evidently.literals import ChangeDirectionEnumType

def get_value() -> ChangeDirectionEnumType:
    return "DECREASE"
```

```python
# ChangeDirectionEnumType definition
ChangeDirectionEnumType = Literal[
    "DECREASE",
    "INCREASE",
]
```
## EventTypeType

```python
# EventTypeType usage example
from types_aiobotocore_evidently.literals import EventTypeType

def get_value() -> EventTypeType:
    return "aws.evidently.custom"
```

```python
# EventTypeType definition
EventTypeType = Literal[
    "aws.evidently.custom",
    "aws.evidently.evaluation",
]
```
## ExperimentBaseStatType

```python
# ExperimentBaseStatType usage example
from types_aiobotocore_evidently.literals import ExperimentBaseStatType

def get_value() -> ExperimentBaseStatType:
    return "Mean"
```

```python
# ExperimentBaseStatType definition
ExperimentBaseStatType = Literal[
    "Mean",
]
```
## ExperimentReportNameType

```python
# ExperimentReportNameType usage example
from types_aiobotocore_evidently.literals import ExperimentReportNameType

def get_value() -> ExperimentReportNameType:
    return "BayesianInference"
```

```python
# ExperimentReportNameType definition
ExperimentReportNameType = Literal[
    "BayesianInference",
]
```
## ExperimentResultRequestTypeType

```python
# ExperimentResultRequestTypeType usage example
from types_aiobotocore_evidently.literals import ExperimentResultRequestTypeType

def get_value() -> ExperimentResultRequestTypeType:
    return "BaseStat"
```

```python
# ExperimentResultRequestTypeType definition
ExperimentResultRequestTypeType = Literal[
    "BaseStat",
    "ConfidenceInterval",
    "PValue",
    "TreatmentEffect",
]
```
## ExperimentResultResponseTypeType

```python
# ExperimentResultResponseTypeType usage example
from types_aiobotocore_evidently.literals import ExperimentResultResponseTypeType

def get_value() -> ExperimentResultResponseTypeType:
    return "ConfidenceIntervalLowerBound"
```

```python
# ExperimentResultResponseTypeType definition
ExperimentResultResponseTypeType = Literal[
    "ConfidenceIntervalLowerBound",
    "ConfidenceIntervalUpperBound",
    "Mean",
    "PValue",
    "TreatmentEffect",
]
```
## ExperimentStatusType

```python
# ExperimentStatusType usage example
from types_aiobotocore_evidently.literals import ExperimentStatusType

def get_value() -> ExperimentStatusType:
    return "CANCELLED"
```

```python
# ExperimentStatusType definition
ExperimentStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "CREATED",
    "RUNNING",
    "UPDATING",
]
```
## ExperimentStopDesiredStateType

```python
# ExperimentStopDesiredStateType usage example
from types_aiobotocore_evidently.literals import ExperimentStopDesiredStateType

def get_value() -> ExperimentStopDesiredStateType:
    return "CANCELLED"
```

```python
# ExperimentStopDesiredStateType definition
ExperimentStopDesiredStateType = Literal[
    "CANCELLED",
    "COMPLETED",
]
```
## ExperimentTypeType

```python
# ExperimentTypeType usage example
from types_aiobotocore_evidently.literals import ExperimentTypeType

def get_value() -> ExperimentTypeType:
    return "aws.evidently.onlineab"
```

```python
# ExperimentTypeType definition
ExperimentTypeType = Literal[
    "aws.evidently.onlineab",
]
```
## FeatureEvaluationStrategyType

```python
# FeatureEvaluationStrategyType usage example
from types_aiobotocore_evidently.literals import FeatureEvaluationStrategyType

def get_value() -> FeatureEvaluationStrategyType:
    return "ALL_RULES"
```

```python
# FeatureEvaluationStrategyType definition
FeatureEvaluationStrategyType = Literal[
    "ALL_RULES",
    "DEFAULT_VARIATION",
]
```
## FeatureStatusType

```python
# FeatureStatusType usage example
from types_aiobotocore_evidently.literals import FeatureStatusType

def get_value() -> FeatureStatusType:
    return "AVAILABLE"
```

```python
# FeatureStatusType definition
FeatureStatusType = Literal[
    "AVAILABLE",
    "UPDATING",
]
```
## LaunchStatusType

```python
# LaunchStatusType usage example
from types_aiobotocore_evidently.literals import LaunchStatusType

def get_value() -> LaunchStatusType:
    return "CANCELLED"
```

```python
# LaunchStatusType definition
LaunchStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "CREATED",
    "RUNNING",
    "UPDATING",
]
```
## LaunchStopDesiredStateType

```python
# LaunchStopDesiredStateType usage example
from types_aiobotocore_evidently.literals import LaunchStopDesiredStateType

def get_value() -> LaunchStopDesiredStateType:
    return "CANCELLED"
```

```python
# LaunchStopDesiredStateType definition
LaunchStopDesiredStateType = Literal[
    "CANCELLED",
    "COMPLETED",
]
```
## LaunchTypeType

```python
# LaunchTypeType usage example
from types_aiobotocore_evidently.literals import LaunchTypeType

def get_value() -> LaunchTypeType:
    return "aws.evidently.splits"
```

```python
# LaunchTypeType definition
LaunchTypeType = Literal[
    "aws.evidently.splits",
]
```
## ListExperimentsPaginatorName

```python
# ListExperimentsPaginatorName usage example
from types_aiobotocore_evidently.literals import ListExperimentsPaginatorName

def get_value() -> ListExperimentsPaginatorName:
    return "list_experiments"
```

```python
# ListExperimentsPaginatorName definition
ListExperimentsPaginatorName = Literal[
    "list_experiments",
]
```
## ListFeaturesPaginatorName

```python
# ListFeaturesPaginatorName usage example
from types_aiobotocore_evidently.literals import ListFeaturesPaginatorName

def get_value() -> ListFeaturesPaginatorName:
    return "list_features"
```

```python
# ListFeaturesPaginatorName definition
ListFeaturesPaginatorName = Literal[
    "list_features",
]
```
## ListLaunchesPaginatorName

```python
# ListLaunchesPaginatorName usage example
from types_aiobotocore_evidently.literals import ListLaunchesPaginatorName

def get_value() -> ListLaunchesPaginatorName:
    return "list_launches"
```

```python
# ListLaunchesPaginatorName definition
ListLaunchesPaginatorName = Literal[
    "list_launches",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example
from types_aiobotocore_evidently.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition
ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ListSegmentReferencesPaginatorName

```python
# ListSegmentReferencesPaginatorName usage example
from types_aiobotocore_evidently.literals import ListSegmentReferencesPaginatorName

def get_value() -> ListSegmentReferencesPaginatorName:
    return "list_segment_references"
```

```python
# ListSegmentReferencesPaginatorName definition
ListSegmentReferencesPaginatorName = Literal[
    "list_segment_references",
]
```
## ListSegmentsPaginatorName

```python
# ListSegmentsPaginatorName usage example
from types_aiobotocore_evidently.literals import ListSegmentsPaginatorName

def get_value() -> ListSegmentsPaginatorName:
    return "list_segments"
```

```python
# ListSegmentsPaginatorName definition
ListSegmentsPaginatorName = Literal[
    "list_segments",
]
```
## ProjectStatusType

```python
# ProjectStatusType usage example
from types_aiobotocore_evidently.literals import ProjectStatusType

def get_value() -> ProjectStatusType:
    return "AVAILABLE"
```

```python
# ProjectStatusType definition
ProjectStatusType = Literal[
    "AVAILABLE",
    "UPDATING",
]
```
## SegmentReferenceResourceTypeType

```python
# SegmentReferenceResourceTypeType usage example
from types_aiobotocore_evidently.literals import SegmentReferenceResourceTypeType

def get_value() -> SegmentReferenceResourceTypeType:
    return "EXPERIMENT"
```

```python
# SegmentReferenceResourceTypeType definition
SegmentReferenceResourceTypeType = Literal[
    "EXPERIMENT",
    "LAUNCH",
]
```
## VariationValueTypeType

```python
# VariationValueTypeType usage example
from types_aiobotocore_evidently.literals import VariationValueTypeType

def get_value() -> VariationValueTypeType:
    return "BOOLEAN"
```

```python
# VariationValueTypeType definition
VariationValueTypeType = Literal[
    "BOOLEAN",
    "DOUBLE",
    "LONG",
    "STRING",
]
```
## CloudWatchEvidentlyServiceName

```python
# CloudWatchEvidentlyServiceName usage example
from types_aiobotocore_evidently.literals import CloudWatchEvidentlyServiceName

def get_value() -> CloudWatchEvidentlyServiceName:
    return "evidently"
```

```python
# CloudWatchEvidentlyServiceName definition
CloudWatchEvidentlyServiceName = Literal[
    "evidently",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_evidently.literals import ServiceName

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
    "compute-optimizer-automation",
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
    "mwaa-serverless",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "nova-act",
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
    "partnercentral-account",
    "partnercentral-benefits",
    "partnercentral-channel",
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
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53globalresolver",
    "route53profiles",
    "route53resolver",
    "rtbfabric",
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
    "signin",
    "simspaceweaver",
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
    "wickr",
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
from types_aiobotocore_evidently.literals import ResourceServiceName

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
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_evidently.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_experiments"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_experiments",
    "list_features",
    "list_launches",
    "list_projects",
    "list_segment_references",
    "list_segments",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_evidently.literals import RegionName

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
