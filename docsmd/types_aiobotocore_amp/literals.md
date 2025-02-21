# Literals

> [Index](../README.md) > [PrometheusService](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## AlertManagerDefinitionStatusCodeType

```python
# AlertManagerDefinitionStatusCodeType usage example
from types_aiobotocore_amp.literals import AlertManagerDefinitionStatusCodeType

def get_value() -> AlertManagerDefinitionStatusCodeType:
    return "ACTIVE"
```

```python
# AlertManagerDefinitionStatusCodeType definition
AlertManagerDefinitionStatusCodeType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ListRuleGroupsNamespacesPaginatorName

```python
# ListRuleGroupsNamespacesPaginatorName usage example
from types_aiobotocore_amp.literals import ListRuleGroupsNamespacesPaginatorName

def get_value() -> ListRuleGroupsNamespacesPaginatorName:
    return "list_rule_groups_namespaces"
```

```python
# ListRuleGroupsNamespacesPaginatorName definition
ListRuleGroupsNamespacesPaginatorName = Literal[
    "list_rule_groups_namespaces",
]
```
## ListScrapersPaginatorName

```python
# ListScrapersPaginatorName usage example
from types_aiobotocore_amp.literals import ListScrapersPaginatorName

def get_value() -> ListScrapersPaginatorName:
    return "list_scrapers"
```

```python
# ListScrapersPaginatorName definition
ListScrapersPaginatorName = Literal[
    "list_scrapers",
]
```
## ListWorkspacesPaginatorName

```python
# ListWorkspacesPaginatorName usage example
from types_aiobotocore_amp.literals import ListWorkspacesPaginatorName

def get_value() -> ListWorkspacesPaginatorName:
    return "list_workspaces"
```

```python
# ListWorkspacesPaginatorName definition
ListWorkspacesPaginatorName = Literal[
    "list_workspaces",
]
```
## LoggingConfigurationStatusCodeType

```python
# LoggingConfigurationStatusCodeType usage example
from types_aiobotocore_amp.literals import LoggingConfigurationStatusCodeType

def get_value() -> LoggingConfigurationStatusCodeType:
    return "ACTIVE"
```

```python
# LoggingConfigurationStatusCodeType definition
LoggingConfigurationStatusCodeType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## RuleGroupsNamespaceStatusCodeType

```python
# RuleGroupsNamespaceStatusCodeType usage example
from types_aiobotocore_amp.literals import RuleGroupsNamespaceStatusCodeType

def get_value() -> RuleGroupsNamespaceStatusCodeType:
    return "ACTIVE"
```

```python
# RuleGroupsNamespaceStatusCodeType definition
RuleGroupsNamespaceStatusCodeType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ScraperActiveWaiterName

```python
# ScraperActiveWaiterName usage example
from types_aiobotocore_amp.literals import ScraperActiveWaiterName

def get_value() -> ScraperActiveWaiterName:
    return "scraper_active"
```

```python
# ScraperActiveWaiterName definition
ScraperActiveWaiterName = Literal[
    "scraper_active",
]
```
## ScraperDeletedWaiterName

```python
# ScraperDeletedWaiterName usage example
from types_aiobotocore_amp.literals import ScraperDeletedWaiterName

def get_value() -> ScraperDeletedWaiterName:
    return "scraper_deleted"
```

```python
# ScraperDeletedWaiterName definition
ScraperDeletedWaiterName = Literal[
    "scraper_deleted",
]
```
## ScraperStatusCodeType

```python
# ScraperStatusCodeType usage example
from types_aiobotocore_amp.literals import ScraperStatusCodeType

def get_value() -> ScraperStatusCodeType:
    return "ACTIVE"
```

```python
# ScraperStatusCodeType definition
ScraperStatusCodeType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "DELETION_FAILED",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## WorkspaceActiveWaiterName

```python
# WorkspaceActiveWaiterName usage example
from types_aiobotocore_amp.literals import WorkspaceActiveWaiterName

def get_value() -> WorkspaceActiveWaiterName:
    return "workspace_active"
```

```python
# WorkspaceActiveWaiterName definition
WorkspaceActiveWaiterName = Literal[
    "workspace_active",
]
```
## WorkspaceDeletedWaiterName

```python
# WorkspaceDeletedWaiterName usage example
from types_aiobotocore_amp.literals import WorkspaceDeletedWaiterName

def get_value() -> WorkspaceDeletedWaiterName:
    return "workspace_deleted"
```

```python
# WorkspaceDeletedWaiterName definition
WorkspaceDeletedWaiterName = Literal[
    "workspace_deleted",
]
```
## WorkspaceStatusCodeType

```python
# WorkspaceStatusCodeType usage example
from types_aiobotocore_amp.literals import WorkspaceStatusCodeType

def get_value() -> WorkspaceStatusCodeType:
    return "ACTIVE"
```

```python
# WorkspaceStatusCodeType definition
WorkspaceStatusCodeType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "UPDATING",
]
```
## PrometheusServiceServiceName

```python
# PrometheusServiceServiceName usage example
from types_aiobotocore_amp.literals import PrometheusServiceServiceName

def get_value() -> PrometheusServiceServiceName:
    return "amp"
```

```python
# PrometheusServiceServiceName definition
PrometheusServiceServiceName = Literal[
    "amp",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_amp.literals import ServiceName

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
from types_aiobotocore_amp.literals import ResourceServiceName

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
from types_aiobotocore_amp.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_rule_groups_namespaces"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_rule_groups_namespaces",
    "list_scrapers",
    "list_workspaces",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_amp.literals import WaiterName

def get_value() -> WaiterName:
    return "scraper_active"
```

```python
# WaiterName definition
WaiterName = Literal[
    "scraper_active",
    "scraper_deleted",
    "workspace_active",
    "workspace_deleted",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_amp.literals import RegionName

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
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
