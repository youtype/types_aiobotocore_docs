# Literals

> [Index](../README.md) > [EventBridge](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## ApiDestinationHttpMethodType

```python
# ApiDestinationHttpMethodType usage example

from types_aiobotocore_events.literals import ApiDestinationHttpMethodType

def get_value() -> ApiDestinationHttpMethodType:
    return "DELETE"
```

```python
# ApiDestinationHttpMethodType definition

ApiDestinationHttpMethodType = Literal[
    "DELETE",
    "GET",
    "HEAD",
    "OPTIONS",
    "PATCH",
    "POST",
    "PUT",
]
```
## ApiDestinationStateType

```python
# ApiDestinationStateType usage example

from types_aiobotocore_events.literals import ApiDestinationStateType

def get_value() -> ApiDestinationStateType:
    return "ACTIVE"
```

```python
# ApiDestinationStateType definition

ApiDestinationStateType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## ArchiveStateType

```python
# ArchiveStateType usage example

from types_aiobotocore_events.literals import ArchiveStateType

def get_value() -> ArchiveStateType:
    return "CREATE_FAILED"
```

```python
# ArchiveStateType definition

ArchiveStateType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DISABLED",
    "ENABLED",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## AssignPublicIpType

```python
# AssignPublicIpType usage example

from types_aiobotocore_events.literals import AssignPublicIpType

def get_value() -> AssignPublicIpType:
    return "DISABLED"
```

```python
# AssignPublicIpType definition

AssignPublicIpType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ConnectionAuthorizationTypeType

```python
# ConnectionAuthorizationTypeType usage example

from types_aiobotocore_events.literals import ConnectionAuthorizationTypeType

def get_value() -> ConnectionAuthorizationTypeType:
    return "API_KEY"
```

```python
# ConnectionAuthorizationTypeType definition

ConnectionAuthorizationTypeType = Literal[
    "API_KEY",
    "BASIC",
    "OAUTH_CLIENT_CREDENTIALS",
]
```
## ConnectionOAuthHttpMethodType

```python
# ConnectionOAuthHttpMethodType usage example

from types_aiobotocore_events.literals import ConnectionOAuthHttpMethodType

def get_value() -> ConnectionOAuthHttpMethodType:
    return "GET"
```

```python
# ConnectionOAuthHttpMethodType definition

ConnectionOAuthHttpMethodType = Literal[
    "GET",
    "POST",
    "PUT",
]
```
## ConnectionStateType

```python
# ConnectionStateType usage example

from types_aiobotocore_events.literals import ConnectionStateType

def get_value() -> ConnectionStateType:
    return "AUTHORIZED"
```

```python
# ConnectionStateType definition

ConnectionStateType = Literal[
    "AUTHORIZED",
    "AUTHORIZING",
    "CREATING",
    "DEAUTHORIZED",
    "DEAUTHORIZING",
    "DELETING",
    "UPDATING",
]
```
## EndpointStateType

```python
# EndpointStateType usage example

from types_aiobotocore_events.literals import EndpointStateType

def get_value() -> EndpointStateType:
    return "ACTIVE"
```

```python
# EndpointStateType definition

EndpointStateType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## EventSourceStateType

```python
# EventSourceStateType usage example

from types_aiobotocore_events.literals import EventSourceStateType

def get_value() -> EventSourceStateType:
    return "ACTIVE"
```

```python
# EventSourceStateType definition

EventSourceStateType = Literal[
    "ACTIVE",
    "DELETED",
    "PENDING",
]
```
## LaunchTypeType

```python
# LaunchTypeType usage example

from types_aiobotocore_events.literals import LaunchTypeType

def get_value() -> LaunchTypeType:
    return "EC2"
```

```python
# LaunchTypeType definition

LaunchTypeType = Literal[
    "EC2",
    "EXTERNAL",
    "FARGATE",
]
```
## ListRuleNamesByTargetPaginatorName

```python
# ListRuleNamesByTargetPaginatorName usage example

from types_aiobotocore_events.literals import ListRuleNamesByTargetPaginatorName

def get_value() -> ListRuleNamesByTargetPaginatorName:
    return "list_rule_names_by_target"
```

```python
# ListRuleNamesByTargetPaginatorName definition

ListRuleNamesByTargetPaginatorName = Literal[
    "list_rule_names_by_target",
]
```
## ListRulesPaginatorName

```python
# ListRulesPaginatorName usage example

from types_aiobotocore_events.literals import ListRulesPaginatorName

def get_value() -> ListRulesPaginatorName:
    return "list_rules"
```

```python
# ListRulesPaginatorName definition

ListRulesPaginatorName = Literal[
    "list_rules",
]
```
## ListTargetsByRulePaginatorName

```python
# ListTargetsByRulePaginatorName usage example

from types_aiobotocore_events.literals import ListTargetsByRulePaginatorName

def get_value() -> ListTargetsByRulePaginatorName:
    return "list_targets_by_rule"
```

```python
# ListTargetsByRulePaginatorName definition

ListTargetsByRulePaginatorName = Literal[
    "list_targets_by_rule",
]
```
## PlacementConstraintTypeType

```python
# PlacementConstraintTypeType usage example

from types_aiobotocore_events.literals import PlacementConstraintTypeType

def get_value() -> PlacementConstraintTypeType:
    return "distinctInstance"
```

```python
# PlacementConstraintTypeType definition

PlacementConstraintTypeType = Literal[
    "distinctInstance",
    "memberOf",
]
```
## PlacementStrategyTypeType

```python
# PlacementStrategyTypeType usage example

from types_aiobotocore_events.literals import PlacementStrategyTypeType

def get_value() -> PlacementStrategyTypeType:
    return "binpack"
```

```python
# PlacementStrategyTypeType definition

PlacementStrategyTypeType = Literal[
    "binpack",
    "random",
    "spread",
]
```
## PropagateTagsType

```python
# PropagateTagsType usage example

from types_aiobotocore_events.literals import PropagateTagsType

def get_value() -> PropagateTagsType:
    return "TASK_DEFINITION"
```

```python
# PropagateTagsType definition

PropagateTagsType = Literal[
    "TASK_DEFINITION",
]
```
## ReplayStateType

```python
# ReplayStateType usage example

from types_aiobotocore_events.literals import ReplayStateType

def get_value() -> ReplayStateType:
    return "CANCELLED"
```

```python
# ReplayStateType definition

ReplayStateType = Literal[
    "CANCELLED",
    "CANCELLING",
    "COMPLETED",
    "FAILED",
    "RUNNING",
    "STARTING",
]
```
## ReplicationStateType

```python
# ReplicationStateType usage example

from types_aiobotocore_events.literals import ReplicationStateType

def get_value() -> ReplicationStateType:
    return "DISABLED"
```

```python
# ReplicationStateType definition

ReplicationStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## RuleStateType

```python
# RuleStateType usage example

from types_aiobotocore_events.literals import RuleStateType

def get_value() -> RuleStateType:
    return "DISABLED"
```

```python
# RuleStateType definition

RuleStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EventBridgeServiceName

```python
# EventBridgeServiceName usage example

from types_aiobotocore_events.literals import EventBridgeServiceName

def get_value() -> EventBridgeServiceName:
    return "events"
```

```python
# EventBridgeServiceName definition

EventBridgeServiceName = Literal[
    "events",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_events.literals import ServiceName

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

from types_aiobotocore_events.literals import ResourceServiceName

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

from types_aiobotocore_events.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_rule_names_by_target"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_rule_names_by_target",
    "list_rules",
    "list_targets_by_rule",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_events.literals import RegionName

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
