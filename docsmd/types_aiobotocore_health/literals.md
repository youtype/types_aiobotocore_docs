# Literals

> [Index](../README.md) > [Health](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## DescribeAffectedAccountsForOrganizationPaginatorName

```python
# DescribeAffectedAccountsForOrganizationPaginatorName usage example

from types_aiobotocore_health.literals import DescribeAffectedAccountsForOrganizationPaginatorName

def get_value() -> DescribeAffectedAccountsForOrganizationPaginatorName:
    return "describe_affected_accounts_for_organization"
```

```python
# DescribeAffectedAccountsForOrganizationPaginatorName definition

DescribeAffectedAccountsForOrganizationPaginatorName = Literal[
    "describe_affected_accounts_for_organization",
]
```
## DescribeAffectedEntitiesForOrganizationPaginatorName

```python
# DescribeAffectedEntitiesForOrganizationPaginatorName usage example

from types_aiobotocore_health.literals import DescribeAffectedEntitiesForOrganizationPaginatorName

def get_value() -> DescribeAffectedEntitiesForOrganizationPaginatorName:
    return "describe_affected_entities_for_organization"
```

```python
# DescribeAffectedEntitiesForOrganizationPaginatorName definition

DescribeAffectedEntitiesForOrganizationPaginatorName = Literal[
    "describe_affected_entities_for_organization",
]
```
## DescribeAffectedEntitiesPaginatorName

```python
# DescribeAffectedEntitiesPaginatorName usage example

from types_aiobotocore_health.literals import DescribeAffectedEntitiesPaginatorName

def get_value() -> DescribeAffectedEntitiesPaginatorName:
    return "describe_affected_entities"
```

```python
# DescribeAffectedEntitiesPaginatorName definition

DescribeAffectedEntitiesPaginatorName = Literal[
    "describe_affected_entities",
]
```
## DescribeEventAggregatesPaginatorName

```python
# DescribeEventAggregatesPaginatorName usage example

from types_aiobotocore_health.literals import DescribeEventAggregatesPaginatorName

def get_value() -> DescribeEventAggregatesPaginatorName:
    return "describe_event_aggregates"
```

```python
# DescribeEventAggregatesPaginatorName definition

DescribeEventAggregatesPaginatorName = Literal[
    "describe_event_aggregates",
]
```
## DescribeEventTypesPaginatorName

```python
# DescribeEventTypesPaginatorName usage example

from types_aiobotocore_health.literals import DescribeEventTypesPaginatorName

def get_value() -> DescribeEventTypesPaginatorName:
    return "describe_event_types"
```

```python
# DescribeEventTypesPaginatorName definition

DescribeEventTypesPaginatorName = Literal[
    "describe_event_types",
]
```
## DescribeEventsForOrganizationPaginatorName

```python
# DescribeEventsForOrganizationPaginatorName usage example

from types_aiobotocore_health.literals import DescribeEventsForOrganizationPaginatorName

def get_value() -> DescribeEventsForOrganizationPaginatorName:
    return "describe_events_for_organization"
```

```python
# DescribeEventsForOrganizationPaginatorName definition

DescribeEventsForOrganizationPaginatorName = Literal[
    "describe_events_for_organization",
]
```
## DescribeEventsPaginatorName

```python
# DescribeEventsPaginatorName usage example

from types_aiobotocore_health.literals import DescribeEventsPaginatorName

def get_value() -> DescribeEventsPaginatorName:
    return "describe_events"
```

```python
# DescribeEventsPaginatorName definition

DescribeEventsPaginatorName = Literal[
    "describe_events",
]
```
## entityStatusCodeType

```python
# entityStatusCodeType usage example

from types_aiobotocore_health.literals import entityStatusCodeType

def get_value() -> entityStatusCodeType:
    return "IMPAIRED"
```

```python
# entityStatusCodeType definition

entityStatusCodeType = Literal[
    "IMPAIRED",
    "UNIMPAIRED",
    "UNKNOWN",
]
```
## eventAggregateFieldType

```python
# eventAggregateFieldType usage example

from types_aiobotocore_health.literals import eventAggregateFieldType

def get_value() -> eventAggregateFieldType:
    return "eventTypeCategory"
```

```python
# eventAggregateFieldType definition

eventAggregateFieldType = Literal[
    "eventTypeCategory",
]
```
## eventScopeCodeType

```python
# eventScopeCodeType usage example

from types_aiobotocore_health.literals import eventScopeCodeType

def get_value() -> eventScopeCodeType:
    return "ACCOUNT_SPECIFIC"
```

```python
# eventScopeCodeType definition

eventScopeCodeType = Literal[
    "ACCOUNT_SPECIFIC",
    "NONE",
    "PUBLIC",
]
```
## eventStatusCodeType

```python
# eventStatusCodeType usage example

from types_aiobotocore_health.literals import eventStatusCodeType

def get_value() -> eventStatusCodeType:
    return "closed"
```

```python
# eventStatusCodeType definition

eventStatusCodeType = Literal[
    "closed",
    "open",
    "upcoming",
]
```
## eventTypeCategoryType

```python
# eventTypeCategoryType usage example

from types_aiobotocore_health.literals import eventTypeCategoryType

def get_value() -> eventTypeCategoryType:
    return "accountNotification"
```

```python
# eventTypeCategoryType definition

eventTypeCategoryType = Literal[
    "accountNotification",
    "investigation",
    "issue",
    "scheduledChange",
]
```
## HealthServiceName

```python
# HealthServiceName usage example

from types_aiobotocore_health.literals import HealthServiceName

def get_value() -> HealthServiceName:
    return "health"
```

```python
# HealthServiceName definition

HealthServiceName = Literal[
    "health",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_health.literals import ServiceName

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

from types_aiobotocore_health.literals import ResourceServiceName

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

from types_aiobotocore_health.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_affected_accounts_for_organization"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_affected_accounts_for_organization",
    "describe_affected_entities",
    "describe_affected_entities_for_organization",
    "describe_event_aggregates",
    "describe_event_types",
    "describe_events",
    "describe_events_for_organization",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_health.literals import RegionName

def get_value() -> RegionName:
    return "us-east-2"
```

```python
# RegionName definition

RegionName = Literal[
    "us-east-2",
]
```
