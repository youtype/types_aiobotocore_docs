# Literals

> [Index](../README.md) > [MediaTailor](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#mediatailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## AccessTypeType

```python
# AccessTypeType usage example

from types_aiobotocore_mediatailor.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "AUTODETECT_SIGV4"
```

```python
# AccessTypeType definition

AccessTypeType = Literal[
    "AUTODETECT_SIGV4",
    "S3_SIGV4",
    "SECRETS_MANAGER_ACCESS_TOKEN",
]
```
## AdMarkupTypeType

```python
# AdMarkupTypeType usage example

from types_aiobotocore_mediatailor.literals import AdMarkupTypeType

def get_value() -> AdMarkupTypeType:
    return "DATERANGE"
```

```python
# AdMarkupTypeType definition

AdMarkupTypeType = Literal[
    "DATERANGE",
    "SCTE35_ENHANCED",
]
```
## AlertCategoryType

```python
# AlertCategoryType usage example

from types_aiobotocore_mediatailor.literals import AlertCategoryType

def get_value() -> AlertCategoryType:
    return "INFO"
```

```python
# AlertCategoryType definition

AlertCategoryType = Literal[
    "INFO",
    "PLAYBACK_WARNING",
    "SCHEDULING_ERROR",
]
```
## ChannelStateType

```python
# ChannelStateType usage example

from types_aiobotocore_mediatailor.literals import ChannelStateType

def get_value() -> ChannelStateType:
    return "RUNNING"
```

```python
# ChannelStateType definition

ChannelStateType = Literal[
    "RUNNING",
    "STOPPED",
]
```
## FillPolicyType

```python
# FillPolicyType usage example

from types_aiobotocore_mediatailor.literals import FillPolicyType

def get_value() -> FillPolicyType:
    return "FULL_AVAIL_ONLY"
```

```python
# FillPolicyType definition

FillPolicyType = Literal[
    "FULL_AVAIL_ONLY",
    "PARTIAL_AVAIL",
]
```
## GetChannelSchedulePaginatorName

```python
# GetChannelSchedulePaginatorName usage example

from types_aiobotocore_mediatailor.literals import GetChannelSchedulePaginatorName

def get_value() -> GetChannelSchedulePaginatorName:
    return "get_channel_schedule"
```

```python
# GetChannelSchedulePaginatorName definition

GetChannelSchedulePaginatorName = Literal[
    "get_channel_schedule",
]
```
## InsertionModeType

```python
# InsertionModeType usage example

from types_aiobotocore_mediatailor.literals import InsertionModeType

def get_value() -> InsertionModeType:
    return "PLAYER_SELECT"
```

```python
# InsertionModeType definition

InsertionModeType = Literal[
    "PLAYER_SELECT",
    "STITCHED_ONLY",
]
```
## ListAlertsPaginatorName

```python
# ListAlertsPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListAlertsPaginatorName

def get_value() -> ListAlertsPaginatorName:
    return "list_alerts"
```

```python
# ListAlertsPaginatorName definition

ListAlertsPaginatorName = Literal[
    "list_alerts",
]
```
## ListChannelsPaginatorName

```python
# ListChannelsPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListChannelsPaginatorName

def get_value() -> ListChannelsPaginatorName:
    return "list_channels"
```

```python
# ListChannelsPaginatorName definition

ListChannelsPaginatorName = Literal[
    "list_channels",
]
```
## ListLiveSourcesPaginatorName

```python
# ListLiveSourcesPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListLiveSourcesPaginatorName

def get_value() -> ListLiveSourcesPaginatorName:
    return "list_live_sources"
```

```python
# ListLiveSourcesPaginatorName definition

ListLiveSourcesPaginatorName = Literal[
    "list_live_sources",
]
```
## ListPlaybackConfigurationsPaginatorName

```python
# ListPlaybackConfigurationsPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListPlaybackConfigurationsPaginatorName

def get_value() -> ListPlaybackConfigurationsPaginatorName:
    return "list_playback_configurations"
```

```python
# ListPlaybackConfigurationsPaginatorName definition

ListPlaybackConfigurationsPaginatorName = Literal[
    "list_playback_configurations",
]
```
## ListPrefetchSchedulesPaginatorName

```python
# ListPrefetchSchedulesPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListPrefetchSchedulesPaginatorName

def get_value() -> ListPrefetchSchedulesPaginatorName:
    return "list_prefetch_schedules"
```

```python
# ListPrefetchSchedulesPaginatorName definition

ListPrefetchSchedulesPaginatorName = Literal[
    "list_prefetch_schedules",
]
```
## ListSourceLocationsPaginatorName

```python
# ListSourceLocationsPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListSourceLocationsPaginatorName

def get_value() -> ListSourceLocationsPaginatorName:
    return "list_source_locations"
```

```python
# ListSourceLocationsPaginatorName definition

ListSourceLocationsPaginatorName = Literal[
    "list_source_locations",
]
```
## ListVodSourcesPaginatorName

```python
# ListVodSourcesPaginatorName usage example

from types_aiobotocore_mediatailor.literals import ListVodSourcesPaginatorName

def get_value() -> ListVodSourcesPaginatorName:
    return "list_vod_sources"
```

```python
# ListVodSourcesPaginatorName definition

ListVodSourcesPaginatorName = Literal[
    "list_vod_sources",
]
```
## LogTypeType

```python
# LogTypeType usage example

from types_aiobotocore_mediatailor.literals import LogTypeType

def get_value() -> LogTypeType:
    return "AS_RUN"
```

```python
# LogTypeType definition

LogTypeType = Literal[
    "AS_RUN",
]
```
## MessageTypeType

```python
# MessageTypeType usage example

from types_aiobotocore_mediatailor.literals import MessageTypeType

def get_value() -> MessageTypeType:
    return "SPLICE_INSERT"
```

```python
# MessageTypeType definition

MessageTypeType = Literal[
    "SPLICE_INSERT",
    "TIME_SIGNAL",
]
```
## ModeType

```python
# ModeType usage example

from types_aiobotocore_mediatailor.literals import ModeType

def get_value() -> ModeType:
    return "AFTER_LIVE_EDGE"
```

```python
# ModeType definition

ModeType = Literal[
    "AFTER_LIVE_EDGE",
    "BEHIND_LIVE_EDGE",
    "OFF",
]
```
## OperatorType

```python
# OperatorType usage example

from types_aiobotocore_mediatailor.literals import OperatorType

def get_value() -> OperatorType:
    return "EQUALS"
```

```python
# OperatorType definition

OperatorType = Literal[
    "EQUALS",
]
```
## OriginManifestTypeType

```python
# OriginManifestTypeType usage example

from types_aiobotocore_mediatailor.literals import OriginManifestTypeType

def get_value() -> OriginManifestTypeType:
    return "MULTI_PERIOD"
```

```python
# OriginManifestTypeType definition

OriginManifestTypeType = Literal[
    "MULTI_PERIOD",
    "SINGLE_PERIOD",
]
```
## PlaybackModeType

```python
# PlaybackModeType usage example

from types_aiobotocore_mediatailor.literals import PlaybackModeType

def get_value() -> PlaybackModeType:
    return "LINEAR"
```

```python
# PlaybackModeType definition

PlaybackModeType = Literal[
    "LINEAR",
    "LOOP",
]
```
## RelativePositionType

```python
# RelativePositionType usage example

from types_aiobotocore_mediatailor.literals import RelativePositionType

def get_value() -> RelativePositionType:
    return "AFTER_PROGRAM"
```

```python
# RelativePositionType definition

RelativePositionType = Literal[
    "AFTER_PROGRAM",
    "BEFORE_PROGRAM",
]
```
## ScheduleEntryTypeType

```python
# ScheduleEntryTypeType usage example

from types_aiobotocore_mediatailor.literals import ScheduleEntryTypeType

def get_value() -> ScheduleEntryTypeType:
    return "ALTERNATE_MEDIA"
```

```python
# ScheduleEntryTypeType definition

ScheduleEntryTypeType = Literal[
    "ALTERNATE_MEDIA",
    "FILLER_SLATE",
    "PROGRAM",
]
```
## TierType

```python
# TierType usage example

from types_aiobotocore_mediatailor.literals import TierType

def get_value() -> TierType:
    return "BASIC"
```

```python
# TierType definition

TierType = Literal[
    "BASIC",
    "STANDARD",
]
```
## TypeType

```python
# TypeType usage example

from types_aiobotocore_mediatailor.literals import TypeType

def get_value() -> TypeType:
    return "DASH"
```

```python
# TypeType definition

TypeType = Literal[
    "DASH",
    "HLS",
]
```
## MediaTailorServiceName

```python
# MediaTailorServiceName usage example

from types_aiobotocore_mediatailor.literals import MediaTailorServiceName

def get_value() -> MediaTailorServiceName:
    return "mediatailor"
```

```python
# MediaTailorServiceName definition

MediaTailorServiceName = Literal[
    "mediatailor",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_mediatailor.literals import ServiceName

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

from types_aiobotocore_mediatailor.literals import ResourceServiceName

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

from types_aiobotocore_mediatailor.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_channel_schedule"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_channel_schedule",
    "list_alerts",
    "list_channels",
    "list_live_sources",
    "list_playback_configurations",
    "list_prefetch_schedules",
    "list_source_locations",
    "list_vod_sources",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_mediatailor.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-4",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-3",
    "me-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
