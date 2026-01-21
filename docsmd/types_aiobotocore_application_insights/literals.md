# Literals

> [Index](../README.md) > [ApplicationInsights](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ApplicationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#applicationinsights)
    type annotations stubs module [types-aiobotocore-application-insights](https://pypi.org/project/types-aiobotocore-application-insights/).

## CloudWatchEventSourceType

```python
# CloudWatchEventSourceType usage example
from types_aiobotocore_application_insights.literals import CloudWatchEventSourceType

def get_value() -> CloudWatchEventSourceType:
    return "CODE_DEPLOY"
```

```python
# CloudWatchEventSourceType definition
CloudWatchEventSourceType = Literal[
    "CODE_DEPLOY",
    "EC2",
    "HEALTH",
    "RDS",
]
```
## ConfigurationEventResourceTypeType

```python
# ConfigurationEventResourceTypeType usage example
from types_aiobotocore_application_insights.literals import ConfigurationEventResourceTypeType

def get_value() -> ConfigurationEventResourceTypeType:
    return "CLOUDFORMATION"
```

```python
# ConfigurationEventResourceTypeType definition
ConfigurationEventResourceTypeType = Literal[
    "CLOUDFORMATION",
    "CLOUDWATCH_ALARM",
    "CLOUDWATCH_LOG",
    "SSM_ASSOCIATION",
]
```
## ConfigurationEventStatusType

```python
# ConfigurationEventStatusType usage example
from types_aiobotocore_application_insights.literals import ConfigurationEventStatusType

def get_value() -> ConfigurationEventStatusType:
    return "ERROR"
```

```python
# ConfigurationEventStatusType definition
ConfigurationEventStatusType = Literal[
    "ERROR",
    "INFO",
    "WARN",
]
```
## DiscoveryTypeType

```python
# DiscoveryTypeType usage example
from types_aiobotocore_application_insights.literals import DiscoveryTypeType

def get_value() -> DiscoveryTypeType:
    return "ACCOUNT_BASED"
```

```python
# DiscoveryTypeType definition
DiscoveryTypeType = Literal[
    "ACCOUNT_BASED",
    "RESOURCE_GROUP_BASED",
]
```
## FeedbackKeyType

```python
# FeedbackKeyType usage example
from types_aiobotocore_application_insights.literals import FeedbackKeyType

def get_value() -> FeedbackKeyType:
    return "INSIGHTS_FEEDBACK"
```

```python
# FeedbackKeyType definition
FeedbackKeyType = Literal[
    "INSIGHTS_FEEDBACK",
]
```
## FeedbackValueType

```python
# FeedbackValueType usage example
from types_aiobotocore_application_insights.literals import FeedbackValueType

def get_value() -> FeedbackValueType:
    return "NOT_SPECIFIED"
```

```python
# FeedbackValueType definition
FeedbackValueType = Literal[
    "NOT_SPECIFIED",
    "NOT_USEFUL",
    "USEFUL",
]
```
## GroupingTypeType

```python
# GroupingTypeType usage example
from types_aiobotocore_application_insights.literals import GroupingTypeType

def get_value() -> GroupingTypeType:
    return "ACCOUNT_BASED"
```

```python
# GroupingTypeType definition
GroupingTypeType = Literal[
    "ACCOUNT_BASED",
]
```
## LogFilterType

```python
# LogFilterType usage example
from types_aiobotocore_application_insights.literals import LogFilterType

def get_value() -> LogFilterType:
    return "ERROR"
```

```python
# LogFilterType definition
LogFilterType = Literal[
    "ERROR",
    "INFO",
    "WARN",
]
```
## OsTypeType

```python
# OsTypeType usage example
from types_aiobotocore_application_insights.literals import OsTypeType

def get_value() -> OsTypeType:
    return "LINUX"
```

```python
# OsTypeType definition
OsTypeType = Literal[
    "LINUX",
    "WINDOWS",
]
```
## RecommendationTypeType

```python
# RecommendationTypeType usage example
from types_aiobotocore_application_insights.literals import RecommendationTypeType

def get_value() -> RecommendationTypeType:
    return "ALL"
```

```python
# RecommendationTypeType definition
RecommendationTypeType = Literal[
    "ALL",
    "INFRA_ONLY",
    "WORKLOAD_ONLY",
]
```
## ResolutionMethodType

```python
# ResolutionMethodType usage example
from types_aiobotocore_application_insights.literals import ResolutionMethodType

def get_value() -> ResolutionMethodType:
    return "AUTOMATIC"
```

```python
# ResolutionMethodType definition
ResolutionMethodType = Literal[
    "AUTOMATIC",
    "MANUAL",
    "UNRESOLVED",
]
```
## SeverityLevelType

```python
# SeverityLevelType usage example
from types_aiobotocore_application_insights.literals import SeverityLevelType

def get_value() -> SeverityLevelType:
    return "High"
```

```python
# SeverityLevelType definition
SeverityLevelType = Literal[
    "High",
    "Informative",
    "Low",
    "Medium",
]
```
## StatusType

```python
# StatusType usage example
from types_aiobotocore_application_insights.literals import StatusType

def get_value() -> StatusType:
    return "IGNORE"
```

```python
# StatusType definition
StatusType = Literal[
    "IGNORE",
    "PENDING",
    "RECOVERING",
    "RECURRING",
    "RESOLVED",
]
```
## TierType

```python
# TierType usage example
from types_aiobotocore_application_insights.literals import TierType

def get_value() -> TierType:
    return "ACTIVE_DIRECTORY"
```

```python
# TierType definition
TierType = Literal[
    "ACTIVE_DIRECTORY",
    "CUSTOM",
    "DEFAULT",
    "DOT_NET_CORE",
    "DOT_NET_WEB",
    "DOT_NET_WEB_TIER",
    "DOT_NET_WORKER",
    "JAVA_JMX",
    "MYSQL",
    "ORACLE",
    "POSTGRESQL",
    "SAP_ASE_HIGH_AVAILABILITY",
    "SAP_ASE_SINGLE_NODE",
    "SAP_HANA_HIGH_AVAILABILITY",
    "SAP_HANA_MULTI_NODE",
    "SAP_HANA_SINGLE_NODE",
    "SAP_NETWEAVER_DISTRIBUTED",
    "SAP_NETWEAVER_HIGH_AVAILABILITY",
    "SAP_NETWEAVER_STANDARD",
    "SHAREPOINT",
    "SQL_SERVER",
    "SQL_SERVER_ALWAYSON_AVAILABILITY_GROUP",
    "SQL_SERVER_FAILOVER_CLUSTER_INSTANCE",
]
```
## UpdateStatusType

```python
# UpdateStatusType usage example
from types_aiobotocore_application_insights.literals import UpdateStatusType

def get_value() -> UpdateStatusType:
    return "RESOLVED"
```

```python
# UpdateStatusType definition
UpdateStatusType = Literal[
    "RESOLVED",
]
```
## VisibilityType

```python
# VisibilityType usage example
from types_aiobotocore_application_insights.literals import VisibilityType

def get_value() -> VisibilityType:
    return "IGNORED"
```

```python
# VisibilityType definition
VisibilityType = Literal[
    "IGNORED",
    "VISIBLE",
]
```
## ApplicationInsightsServiceName

```python
# ApplicationInsightsServiceName usage example
from types_aiobotocore_application_insights.literals import ApplicationInsightsServiceName

def get_value() -> ApplicationInsightsServiceName:
    return "application-insights"
```

```python
# ApplicationInsightsServiceName definition
ApplicationInsightsServiceName = Literal[
    "application-insights",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_application_insights.literals import ServiceName

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
from types_aiobotocore_application_insights.literals import ResourceServiceName

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
from types_aiobotocore_application_insights.literals import RegionName

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
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
