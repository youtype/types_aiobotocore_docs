# Literals

> [Index](../README.md) > [MediaConnect](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## AlgorithmType

```python
# AlgorithmType usage example

from types_aiobotocore_mediaconnect.literals import AlgorithmType

def get_value() -> AlgorithmType:
    return "aes128"
```

```python
# AlgorithmType definition

AlgorithmType = Literal[
    "aes128",
    "aes192",
    "aes256",
]
```
## BridgePlacementType

```python
# BridgePlacementType usage example

from types_aiobotocore_mediaconnect.literals import BridgePlacementType

def get_value() -> BridgePlacementType:
    return "AVAILABLE"
```

```python
# BridgePlacementType definition

BridgePlacementType = Literal[
    "AVAILABLE",
    "LOCKED",
]
```
## BridgeStateType

```python
# BridgeStateType usage example

from types_aiobotocore_mediaconnect.literals import BridgeStateType

def get_value() -> BridgeStateType:
    return "ACTIVE"
```

```python
# BridgeStateType definition

BridgeStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETED",
    "DELETING",
    "DEPLOYING",
    "STANDBY",
    "START_FAILED",
    "START_PENDING",
    "STARTING",
    "STOP_FAILED",
    "STOPPING",
    "UPDATING",
]
```
## ColorimetryType

```python
# ColorimetryType usage example

from types_aiobotocore_mediaconnect.literals import ColorimetryType

def get_value() -> ColorimetryType:
    return "BT2020"
```

```python
# ColorimetryType definition

ColorimetryType = Literal[
    "BT2020",
    "BT2100",
    "BT601",
    "BT709",
    "ST2065-1",
    "ST2065-3",
    "XYZ",
]
```
## ConnectionStatusType

```python
# ConnectionStatusType usage example

from types_aiobotocore_mediaconnect.literals import ConnectionStatusType

def get_value() -> ConnectionStatusType:
    return "CONNECTED"
```

```python
# ConnectionStatusType definition

ConnectionStatusType = Literal[
    "CONNECTED",
    "DISCONNECTED",
]
```
## ContentQualityAnalysisStateType

```python
# ContentQualityAnalysisStateType usage example

from types_aiobotocore_mediaconnect.literals import ContentQualityAnalysisStateType

def get_value() -> ContentQualityAnalysisStateType:
    return "DISABLED"
```

```python
# ContentQualityAnalysisStateType definition

ContentQualityAnalysisStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## DesiredStateType

```python
# DesiredStateType usage example

from types_aiobotocore_mediaconnect.literals import DesiredStateType

def get_value() -> DesiredStateType:
    return "ACTIVE"
```

```python
# DesiredStateType definition

DesiredStateType = Literal[
    "ACTIVE",
    "DELETED",
    "STANDBY",
]
```
## DurationUnitsType

```python
# DurationUnitsType usage example

from types_aiobotocore_mediaconnect.literals import DurationUnitsType

def get_value() -> DurationUnitsType:
    return "MONTHS"
```

```python
# DurationUnitsType definition

DurationUnitsType = Literal[
    "MONTHS",
]
```
## EncoderProfileType

```python
# EncoderProfileType usage example

from types_aiobotocore_mediaconnect.literals import EncoderProfileType

def get_value() -> EncoderProfileType:
    return "high"
```

```python
# EncoderProfileType definition

EncoderProfileType = Literal[
    "high",
    "main",
]
```
## EncodingNameType

```python
# EncodingNameType usage example

from types_aiobotocore_mediaconnect.literals import EncodingNameType

def get_value() -> EncodingNameType:
    return "jxsv"
```

```python
# EncodingNameType definition

EncodingNameType = Literal[
    "jxsv",
    "pcm",
    "raw",
    "smpte291",
]
```
## EntitlementStatusType

```python
# EntitlementStatusType usage example

from types_aiobotocore_mediaconnect.literals import EntitlementStatusType

def get_value() -> EntitlementStatusType:
    return "DISABLED"
```

```python
# EntitlementStatusType definition

EntitlementStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## FailoverModeType

```python
# FailoverModeType usage example

from types_aiobotocore_mediaconnect.literals import FailoverModeType

def get_value() -> FailoverModeType:
    return "FAILOVER"
```

```python
# FailoverModeType definition

FailoverModeType = Literal[
    "FAILOVER",
    "MERGE",
]
```
## FlowActiveWaiterName

```python
# FlowActiveWaiterName usage example

from types_aiobotocore_mediaconnect.literals import FlowActiveWaiterName

def get_value() -> FlowActiveWaiterName:
    return "flow_active"
```

```python
# FlowActiveWaiterName definition

FlowActiveWaiterName = Literal[
    "flow_active",
]
```
## FlowDeletedWaiterName

```python
# FlowDeletedWaiterName usage example

from types_aiobotocore_mediaconnect.literals import FlowDeletedWaiterName

def get_value() -> FlowDeletedWaiterName:
    return "flow_deleted"
```

```python
# FlowDeletedWaiterName definition

FlowDeletedWaiterName = Literal[
    "flow_deleted",
]
```
## FlowStandbyWaiterName

```python
# FlowStandbyWaiterName usage example

from types_aiobotocore_mediaconnect.literals import FlowStandbyWaiterName

def get_value() -> FlowStandbyWaiterName:
    return "flow_standby"
```

```python
# FlowStandbyWaiterName definition

FlowStandbyWaiterName = Literal[
    "flow_standby",
]
```
## GatewayStateType

```python
# GatewayStateType usage example

from types_aiobotocore_mediaconnect.literals import GatewayStateType

def get_value() -> GatewayStateType:
    return "ACTIVE"
```

```python
# GatewayStateType definition

GatewayStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETED",
    "DELETING",
    "ERROR",
    "UPDATING",
]
```
## InstanceStateType

```python
# InstanceStateType usage example

from types_aiobotocore_mediaconnect.literals import InstanceStateType

def get_value() -> InstanceStateType:
    return "ACTIVE"
```

```python
# InstanceStateType definition

InstanceStateType = Literal[
    "ACTIVE",
    "DEREGISTERED",
    "DEREGISTERING",
    "DEREGISTRATION_ERROR",
    "REGISTERING",
    "REGISTRATION_ERROR",
]
```
## KeyTypeType

```python
# KeyTypeType usage example

from types_aiobotocore_mediaconnect.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "speke"
```

```python
# KeyTypeType definition

KeyTypeType = Literal[
    "speke",
    "srt-password",
    "static-key",
]
```
## ListBridgesPaginatorName

```python
# ListBridgesPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListBridgesPaginatorName

def get_value() -> ListBridgesPaginatorName:
    return "list_bridges"
```

```python
# ListBridgesPaginatorName definition

ListBridgesPaginatorName = Literal[
    "list_bridges",
]
```
## ListEntitlementsPaginatorName

```python
# ListEntitlementsPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListEntitlementsPaginatorName

def get_value() -> ListEntitlementsPaginatorName:
    return "list_entitlements"
```

```python
# ListEntitlementsPaginatorName definition

ListEntitlementsPaginatorName = Literal[
    "list_entitlements",
]
```
## ListFlowsPaginatorName

```python
# ListFlowsPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListFlowsPaginatorName

def get_value() -> ListFlowsPaginatorName:
    return "list_flows"
```

```python
# ListFlowsPaginatorName definition

ListFlowsPaginatorName = Literal[
    "list_flows",
]
```
## ListGatewayInstancesPaginatorName

```python
# ListGatewayInstancesPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListGatewayInstancesPaginatorName

def get_value() -> ListGatewayInstancesPaginatorName:
    return "list_gateway_instances"
```

```python
# ListGatewayInstancesPaginatorName definition

ListGatewayInstancesPaginatorName = Literal[
    "list_gateway_instances",
]
```
## ListGatewaysPaginatorName

```python
# ListGatewaysPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListGatewaysPaginatorName

def get_value() -> ListGatewaysPaginatorName:
    return "list_gateways"
```

```python
# ListGatewaysPaginatorName definition

ListGatewaysPaginatorName = Literal[
    "list_gateways",
]
```
## ListOfferingsPaginatorName

```python
# ListOfferingsPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListOfferingsPaginatorName

def get_value() -> ListOfferingsPaginatorName:
    return "list_offerings"
```

```python
# ListOfferingsPaginatorName definition

ListOfferingsPaginatorName = Literal[
    "list_offerings",
]
```
## ListReservationsPaginatorName

```python
# ListReservationsPaginatorName usage example

from types_aiobotocore_mediaconnect.literals import ListReservationsPaginatorName

def get_value() -> ListReservationsPaginatorName:
    return "list_reservations"
```

```python
# ListReservationsPaginatorName definition

ListReservationsPaginatorName = Literal[
    "list_reservations",
]
```
## MaintenanceDayType

```python
# MaintenanceDayType usage example

from types_aiobotocore_mediaconnect.literals import MaintenanceDayType

def get_value() -> MaintenanceDayType:
    return "Friday"
```

```python
# MaintenanceDayType definition

MaintenanceDayType = Literal[
    "Friday",
    "Monday",
    "Saturday",
    "Sunday",
    "Thursday",
    "Tuesday",
    "Wednesday",
]
```
## MediaStreamTypeType

```python
# MediaStreamTypeType usage example

from types_aiobotocore_mediaconnect.literals import MediaStreamTypeType

def get_value() -> MediaStreamTypeType:
    return "ancillary-data"
```

```python
# MediaStreamTypeType definition

MediaStreamTypeType = Literal[
    "ancillary-data",
    "audio",
    "video",
]
```
## NetworkInterfaceTypeType

```python
# NetworkInterfaceTypeType usage example

from types_aiobotocore_mediaconnect.literals import NetworkInterfaceTypeType

def get_value() -> NetworkInterfaceTypeType:
    return "efa"
```

```python
# NetworkInterfaceTypeType definition

NetworkInterfaceTypeType = Literal[
    "efa",
    "ena",
]
```
## OutputStatusType

```python
# OutputStatusType usage example

from types_aiobotocore_mediaconnect.literals import OutputStatusType

def get_value() -> OutputStatusType:
    return "DISABLED"
```

```python
# OutputStatusType definition

OutputStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PriceUnitsType

```python
# PriceUnitsType usage example

from types_aiobotocore_mediaconnect.literals import PriceUnitsType

def get_value() -> PriceUnitsType:
    return "HOURLY"
```

```python
# PriceUnitsType definition

PriceUnitsType = Literal[
    "HOURLY",
]
```
## ProtocolType

```python
# ProtocolType usage example

from types_aiobotocore_mediaconnect.literals import ProtocolType

def get_value() -> ProtocolType:
    return "cdi"
```

```python
# ProtocolType definition

ProtocolType = Literal[
    "cdi",
    "fujitsu-qos",
    "rist",
    "rtp",
    "rtp-fec",
    "srt-caller",
    "srt-listener",
    "st2110-jpegxs",
    "udp",
    "zixi-pull",
    "zixi-push",
]
```
## RangeType

```python
# RangeType usage example

from types_aiobotocore_mediaconnect.literals import RangeType

def get_value() -> RangeType:
    return "FULL"
```

```python
# RangeType definition

RangeType = Literal[
    "FULL",
    "FULLPROTECT",
    "NARROW",
]
```
## ReservationStateType

```python
# ReservationStateType usage example

from types_aiobotocore_mediaconnect.literals import ReservationStateType

def get_value() -> ReservationStateType:
    return "ACTIVE"
```

```python
# ReservationStateType definition

ReservationStateType = Literal[
    "ACTIVE",
    "CANCELED",
    "EXPIRED",
    "PROCESSING",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example

from types_aiobotocore_mediaconnect.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "Mbps_Outbound_Bandwidth"
```

```python
# ResourceTypeType definition

ResourceTypeType = Literal[
    "Mbps_Outbound_Bandwidth",
]
```
## ScanModeType

```python
# ScanModeType usage example

from types_aiobotocore_mediaconnect.literals import ScanModeType

def get_value() -> ScanModeType:
    return "interlace"
```

```python
# ScanModeType definition

ScanModeType = Literal[
    "interlace",
    "progressive",
    "progressive-segmented-frame",
]
```
## SourceTypeType

```python
# SourceTypeType usage example

from types_aiobotocore_mediaconnect.literals import SourceTypeType

def get_value() -> SourceTypeType:
    return "ENTITLED"
```

```python
# SourceTypeType definition

SourceTypeType = Literal[
    "ENTITLED",
    "OWNED",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_mediaconnect.literals import StateType

def get_value() -> StateType:
    return "DISABLED"
```

```python
# StateType definition

StateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## StatusType

```python
# StatusType usage example

from types_aiobotocore_mediaconnect.literals import StatusType

def get_value() -> StatusType:
    return "ACTIVE"
```

```python
# StatusType definition

StatusType = Literal[
    "ACTIVE",
    "DELETING",
    "ERROR",
    "STANDBY",
    "STARTING",
    "STOPPING",
    "UPDATING",
]
```
## TcsType

```python
# TcsType usage example

from types_aiobotocore_mediaconnect.literals import TcsType

def get_value() -> TcsType:
    return "BT2100LINHLG"
```

```python
# TcsType definition

TcsType = Literal[
    "BT2100LINHLG",
    "BT2100LINPQ",
    "DENSITY",
    "HLG",
    "LINEAR",
    "PQ",
    "SDR",
    "ST2065-1",
    "ST428-1",
]
```
## ThumbnailStateType

```python
# ThumbnailStateType usage example

from types_aiobotocore_mediaconnect.literals import ThumbnailStateType

def get_value() -> ThumbnailStateType:
    return "DISABLED"
```

```python
# ThumbnailStateType definition

ThumbnailStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## MediaConnectServiceName

```python
# MediaConnectServiceName usage example

from types_aiobotocore_mediaconnect.literals import MediaConnectServiceName

def get_value() -> MediaConnectServiceName:
    return "mediaconnect"
```

```python
# MediaConnectServiceName definition

MediaConnectServiceName = Literal[
    "mediaconnect",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_mediaconnect.literals import ServiceName

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

from types_aiobotocore_mediaconnect.literals import ResourceServiceName

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

from types_aiobotocore_mediaconnect.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_bridges"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_bridges",
    "list_entitlements",
    "list_flows",
    "list_gateway_instances",
    "list_gateways",
    "list_offerings",
    "list_reservations",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_mediaconnect.literals import WaiterName

def get_value() -> WaiterName:
    return "flow_active"
```

```python
# WaiterName definition

WaiterName = Literal[
    "flow_active",
    "flow_deleted",
    "flow_standby",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_mediaconnect.literals import RegionName

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
    "ap-southeast-4",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
