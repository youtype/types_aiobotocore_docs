# Literals

> [Index](../README.md) > [Outposts](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## AddressTypeType

```python
# AddressTypeType usage example

from types_aiobotocore_outposts.literals import AddressTypeType

def get_value() -> AddressTypeType:
    return "OPERATING_ADDRESS"
```

```python
# AddressTypeType definition

AddressTypeType = Literal[
    "OPERATING_ADDRESS",
    "SHIPPING_ADDRESS",
]
```
## AssetStateType

```python
# AssetStateType usage example

from types_aiobotocore_outposts.literals import AssetStateType

def get_value() -> AssetStateType:
    return "ACTIVE"
```

```python
# AssetStateType definition

AssetStateType = Literal[
    "ACTIVE",
    "ISOLATED",
    "RETIRING",
]
```
## AssetTypeType

```python
# AssetTypeType usage example

from types_aiobotocore_outposts.literals import AssetTypeType

def get_value() -> AssetTypeType:
    return "COMPUTE"
```

```python
# AssetTypeType definition

AssetTypeType = Literal[
    "COMPUTE",
]
```
## CatalogItemClassType

```python
# CatalogItemClassType usage example

from types_aiobotocore_outposts.literals import CatalogItemClassType

def get_value() -> CatalogItemClassType:
    return "RACK"
```

```python
# CatalogItemClassType definition

CatalogItemClassType = Literal[
    "RACK",
    "SERVER",
]
```
## CatalogItemStatusType

```python
# CatalogItemStatusType usage example

from types_aiobotocore_outposts.literals import CatalogItemStatusType

def get_value() -> CatalogItemStatusType:
    return "AVAILABLE"
```

```python
# CatalogItemStatusType definition

CatalogItemStatusType = Literal[
    "AVAILABLE",
    "DISCONTINUED",
]
```
## ComputeAssetStateType

```python
# ComputeAssetStateType usage example

from types_aiobotocore_outposts.literals import ComputeAssetStateType

def get_value() -> ComputeAssetStateType:
    return "ACTIVE"
```

```python
# ComputeAssetStateType definition

ComputeAssetStateType = Literal[
    "ACTIVE",
    "ISOLATED",
    "RETIRING",
]
```
## FiberOpticCableTypeType

```python
# FiberOpticCableTypeType usage example

from types_aiobotocore_outposts.literals import FiberOpticCableTypeType

def get_value() -> FiberOpticCableTypeType:
    return "MULTI_MODE"
```

```python
# FiberOpticCableTypeType definition

FiberOpticCableTypeType = Literal[
    "MULTI_MODE",
    "SINGLE_MODE",
]
```
## GetOutpostInstanceTypesPaginatorName

```python
# GetOutpostInstanceTypesPaginatorName usage example

from types_aiobotocore_outposts.literals import GetOutpostInstanceTypesPaginatorName

def get_value() -> GetOutpostInstanceTypesPaginatorName:
    return "get_outpost_instance_types"
```

```python
# GetOutpostInstanceTypesPaginatorName definition

GetOutpostInstanceTypesPaginatorName = Literal[
    "get_outpost_instance_types",
]
```
## LineItemStatusType

```python
# LineItemStatusType usage example

from types_aiobotocore_outposts.literals import LineItemStatusType

def get_value() -> LineItemStatusType:
    return "BUILDING"
```

```python
# LineItemStatusType definition

LineItemStatusType = Literal[
    "BUILDING",
    "CANCELLED",
    "DELIVERED",
    "ERROR",
    "INSTALLED",
    "INSTALLING",
    "PREPARING",
    "REPLACED",
    "SHIPPED",
]
```
## ListAssetsPaginatorName

```python
# ListAssetsPaginatorName usage example

from types_aiobotocore_outposts.literals import ListAssetsPaginatorName

def get_value() -> ListAssetsPaginatorName:
    return "list_assets"
```

```python
# ListAssetsPaginatorName definition

ListAssetsPaginatorName = Literal[
    "list_assets",
]
```
## ListCatalogItemsPaginatorName

```python
# ListCatalogItemsPaginatorName usage example

from types_aiobotocore_outposts.literals import ListCatalogItemsPaginatorName

def get_value() -> ListCatalogItemsPaginatorName:
    return "list_catalog_items"
```

```python
# ListCatalogItemsPaginatorName definition

ListCatalogItemsPaginatorName = Literal[
    "list_catalog_items",
]
```
## ListOrdersPaginatorName

```python
# ListOrdersPaginatorName usage example

from types_aiobotocore_outposts.literals import ListOrdersPaginatorName

def get_value() -> ListOrdersPaginatorName:
    return "list_orders"
```

```python
# ListOrdersPaginatorName definition

ListOrdersPaginatorName = Literal[
    "list_orders",
]
```
## ListOutpostsPaginatorName

```python
# ListOutpostsPaginatorName usage example

from types_aiobotocore_outposts.literals import ListOutpostsPaginatorName

def get_value() -> ListOutpostsPaginatorName:
    return "list_outposts"
```

```python
# ListOutpostsPaginatorName definition

ListOutpostsPaginatorName = Literal[
    "list_outposts",
]
```
## ListSitesPaginatorName

```python
# ListSitesPaginatorName usage example

from types_aiobotocore_outposts.literals import ListSitesPaginatorName

def get_value() -> ListSitesPaginatorName:
    return "list_sites"
```

```python
# ListSitesPaginatorName definition

ListSitesPaginatorName = Literal[
    "list_sites",
]
```
## MaximumSupportedWeightLbsType

```python
# MaximumSupportedWeightLbsType usage example

from types_aiobotocore_outposts.literals import MaximumSupportedWeightLbsType

def get_value() -> MaximumSupportedWeightLbsType:
    return "MAX_1400_LBS"
```

```python
# MaximumSupportedWeightLbsType definition

MaximumSupportedWeightLbsType = Literal[
    "MAX_1400_LBS",
    "MAX_1600_LBS",
    "MAX_1800_LBS",
    "MAX_2000_LBS",
    "NO_LIMIT",
]
```
## OpticalStandardType

```python
# OpticalStandardType usage example

from types_aiobotocore_outposts.literals import OpticalStandardType

def get_value() -> OpticalStandardType:
    return "OPTIC_1000BASE_LX"
```

```python
# OpticalStandardType definition

OpticalStandardType = Literal[
    "OPTIC_1000BASE_LX",
    "OPTIC_1000BASE_SX",
    "OPTIC_100G_PSM4_MSA",
    "OPTIC_100GBASE_CWDM4",
    "OPTIC_100GBASE_LR4",
    "OPTIC_100GBASE_SR4",
    "OPTIC_10GBASE_IR",
    "OPTIC_10GBASE_LR",
    "OPTIC_10GBASE_SR",
    "OPTIC_40GBASE_ESR",
    "OPTIC_40GBASE_IR4_LR4L",
    "OPTIC_40GBASE_LR4",
    "OPTIC_40GBASE_SR",
]
```
## OrderStatusType

```python
# OrderStatusType usage example

from types_aiobotocore_outposts.literals import OrderStatusType

def get_value() -> OrderStatusType:
    return "CANCELLED"
```

```python
# OrderStatusType definition

OrderStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "ERROR",
    "FULFILLED",
    "IN_PROGRESS",
    "INSTALLING",
    "PENDING",
    "PREPARING",
    "PROCESSING",
    "RECEIVED",
]
```
## OrderTypeType

```python
# OrderTypeType usage example

from types_aiobotocore_outposts.literals import OrderTypeType

def get_value() -> OrderTypeType:
    return "OUTPOST"
```

```python
# OrderTypeType definition

OrderTypeType = Literal[
    "OUTPOST",
    "REPLACEMENT",
]
```
## PaymentOptionType

```python
# PaymentOptionType usage example

from types_aiobotocore_outposts.literals import PaymentOptionType

def get_value() -> PaymentOptionType:
    return "ALL_UPFRONT"
```

```python
# PaymentOptionType definition

PaymentOptionType = Literal[
    "ALL_UPFRONT",
    "NO_UPFRONT",
    "PARTIAL_UPFRONT",
]
```
## PaymentTermType

```python
# PaymentTermType usage example

from types_aiobotocore_outposts.literals import PaymentTermType

def get_value() -> PaymentTermType:
    return "ONE_YEAR"
```

```python
# PaymentTermType definition

PaymentTermType = Literal[
    "ONE_YEAR",
    "THREE_YEARS",
]
```
## PowerConnectorType

```python
# PowerConnectorType usage example

from types_aiobotocore_outposts.literals import PowerConnectorType

def get_value() -> PowerConnectorType:
    return "AH530P7W"
```

```python
# PowerConnectorType definition

PowerConnectorType = Literal[
    "AH530P7W",
    "AH532P6W",
    "IEC309",
    "L6_30P",
]
```
## PowerDrawKvaType

```python
# PowerDrawKvaType usage example

from types_aiobotocore_outposts.literals import PowerDrawKvaType

def get_value() -> PowerDrawKvaType:
    return "POWER_10_KVA"
```

```python
# PowerDrawKvaType definition

PowerDrawKvaType = Literal[
    "POWER_10_KVA",
    "POWER_15_KVA",
    "POWER_30_KVA",
    "POWER_5_KVA",
]
```
## PowerFeedDropType

```python
# PowerFeedDropType usage example

from types_aiobotocore_outposts.literals import PowerFeedDropType

def get_value() -> PowerFeedDropType:
    return "ABOVE_RACK"
```

```python
# PowerFeedDropType definition

PowerFeedDropType = Literal[
    "ABOVE_RACK",
    "BELOW_RACK",
]
```
## PowerPhaseType

```python
# PowerPhaseType usage example

from types_aiobotocore_outposts.literals import PowerPhaseType

def get_value() -> PowerPhaseType:
    return "SINGLE_PHASE"
```

```python
# PowerPhaseType definition

PowerPhaseType = Literal[
    "SINGLE_PHASE",
    "THREE_PHASE",
]
```
## ShipmentCarrierType

```python
# ShipmentCarrierType usage example

from types_aiobotocore_outposts.literals import ShipmentCarrierType

def get_value() -> ShipmentCarrierType:
    return "DBS"
```

```python
# ShipmentCarrierType definition

ShipmentCarrierType = Literal[
    "DBS",
    "DHL",
    "FEDEX",
    "UPS",
]
```
## SupportedHardwareTypeType

```python
# SupportedHardwareTypeType usage example

from types_aiobotocore_outposts.literals import SupportedHardwareTypeType

def get_value() -> SupportedHardwareTypeType:
    return "RACK"
```

```python
# SupportedHardwareTypeType definition

SupportedHardwareTypeType = Literal[
    "RACK",
    "SERVER",
]
```
## SupportedStorageEnumType

```python
# SupportedStorageEnumType usage example

from types_aiobotocore_outposts.literals import SupportedStorageEnumType

def get_value() -> SupportedStorageEnumType:
    return "EBS"
```

```python
# SupportedStorageEnumType definition

SupportedStorageEnumType = Literal[
    "EBS",
    "S3",
]
```
## UplinkCountType

```python
# UplinkCountType usage example

from types_aiobotocore_outposts.literals import UplinkCountType

def get_value() -> UplinkCountType:
    return "UPLINK_COUNT_1"
```

```python
# UplinkCountType definition

UplinkCountType = Literal[
    "UPLINK_COUNT_1",
    "UPLINK_COUNT_12",
    "UPLINK_COUNT_16",
    "UPLINK_COUNT_2",
    "UPLINK_COUNT_3",
    "UPLINK_COUNT_4",
    "UPLINK_COUNT_5",
    "UPLINK_COUNT_6",
    "UPLINK_COUNT_7",
    "UPLINK_COUNT_8",
]
```
## UplinkGbpsType

```python
# UplinkGbpsType usage example

from types_aiobotocore_outposts.literals import UplinkGbpsType

def get_value() -> UplinkGbpsType:
    return "UPLINK_100G"
```

```python
# UplinkGbpsType definition

UplinkGbpsType = Literal[
    "UPLINK_100G",
    "UPLINK_10G",
    "UPLINK_1G",
    "UPLINK_40G",
]
```
## OutpostsServiceName

```python
# OutpostsServiceName usage example

from types_aiobotocore_outposts.literals import OutpostsServiceName

def get_value() -> OutpostsServiceName:
    return "outposts"
```

```python
# OutpostsServiceName definition

OutpostsServiceName = Literal[
    "outposts",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_outposts.literals import ServiceName

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

from types_aiobotocore_outposts.literals import ResourceServiceName

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

from types_aiobotocore_outposts.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_outpost_instance_types"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_outpost_instance_types",
    "list_assets",
    "list_catalog_items",
    "list_orders",
    "list_outposts",
    "list_sites",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_outposts.literals import RegionName

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
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
