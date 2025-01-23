# Literals

> [Index](../README.md) > [Private5G](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#private5g)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## AcknowledgmentStatusType

```python
# AcknowledgmentStatusType usage example

from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType

def get_value() -> AcknowledgmentStatusType:
    return "ACKNOWLEDGED"
```

```python
# AcknowledgmentStatusType definition

AcknowledgmentStatusType = Literal[
    "ACKNOWLEDGED",
    "ACKNOWLEDGING",
    "UNACKNOWLEDGED",
]
```
## CommitmentLengthType

```python
# CommitmentLengthType usage example

from types_aiobotocore_privatenetworks.literals import CommitmentLengthType

def get_value() -> CommitmentLengthType:
    return "ONE_YEAR"
```

```python
# CommitmentLengthType definition

CommitmentLengthType = Literal[
    "ONE_YEAR",
    "SIXTY_DAYS",
    "THREE_YEARS",
]
```
## DeviceIdentifierFilterKeysType

```python
# DeviceIdentifierFilterKeysType usage example

from types_aiobotocore_privatenetworks.literals import DeviceIdentifierFilterKeysType

def get_value() -> DeviceIdentifierFilterKeysType:
    return "ORDER"
```

```python
# DeviceIdentifierFilterKeysType definition

DeviceIdentifierFilterKeysType = Literal[
    "ORDER",
    "STATUS",
    "TRAFFIC_GROUP",
]
```
## DeviceIdentifierStatusType

```python
# DeviceIdentifierStatusType usage example

from types_aiobotocore_privatenetworks.literals import DeviceIdentifierStatusType

def get_value() -> DeviceIdentifierStatusType:
    return "ACTIVE"
```

```python
# DeviceIdentifierStatusType definition

DeviceIdentifierStatusType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## ElevationReferenceType

```python
# ElevationReferenceType usage example

from types_aiobotocore_privatenetworks.literals import ElevationReferenceType

def get_value() -> ElevationReferenceType:
    return "AGL"
```

```python
# ElevationReferenceType definition

ElevationReferenceType = Literal[
    "AGL",
    "AMSL",
]
```
## ElevationUnitType

```python
# ElevationUnitType usage example

from types_aiobotocore_privatenetworks.literals import ElevationUnitType

def get_value() -> ElevationUnitType:
    return "FEET"
```

```python
# ElevationUnitType definition

ElevationUnitType = Literal[
    "FEET",
]
```
## HealthStatusType

```python
# HealthStatusType usage example

from types_aiobotocore_privatenetworks.literals import HealthStatusType

def get_value() -> HealthStatusType:
    return "HEALTHY"
```

```python
# HealthStatusType definition

HealthStatusType = Literal[
    "HEALTHY",
    "INITIAL",
    "UNHEALTHY",
]
```
## ListDeviceIdentifiersPaginatorName

```python
# ListDeviceIdentifiersPaginatorName usage example

from types_aiobotocore_privatenetworks.literals import ListDeviceIdentifiersPaginatorName

def get_value() -> ListDeviceIdentifiersPaginatorName:
    return "list_device_identifiers"
```

```python
# ListDeviceIdentifiersPaginatorName definition

ListDeviceIdentifiersPaginatorName = Literal[
    "list_device_identifiers",
]
```
## ListNetworkResourcesPaginatorName

```python
# ListNetworkResourcesPaginatorName usage example

from types_aiobotocore_privatenetworks.literals import ListNetworkResourcesPaginatorName

def get_value() -> ListNetworkResourcesPaginatorName:
    return "list_network_resources"
```

```python
# ListNetworkResourcesPaginatorName definition

ListNetworkResourcesPaginatorName = Literal[
    "list_network_resources",
]
```
## ListNetworkSitesPaginatorName

```python
# ListNetworkSitesPaginatorName usage example

from types_aiobotocore_privatenetworks.literals import ListNetworkSitesPaginatorName

def get_value() -> ListNetworkSitesPaginatorName:
    return "list_network_sites"
```

```python
# ListNetworkSitesPaginatorName definition

ListNetworkSitesPaginatorName = Literal[
    "list_network_sites",
]
```
## ListNetworksPaginatorName

```python
# ListNetworksPaginatorName usage example

from types_aiobotocore_privatenetworks.literals import ListNetworksPaginatorName

def get_value() -> ListNetworksPaginatorName:
    return "list_networks"
```

```python
# ListNetworksPaginatorName definition

ListNetworksPaginatorName = Literal[
    "list_networks",
]
```
## ListOrdersPaginatorName

```python
# ListOrdersPaginatorName usage example

from types_aiobotocore_privatenetworks.literals import ListOrdersPaginatorName

def get_value() -> ListOrdersPaginatorName:
    return "list_orders"
```

```python
# ListOrdersPaginatorName definition

ListOrdersPaginatorName = Literal[
    "list_orders",
]
```
## NetworkFilterKeysType

```python
# NetworkFilterKeysType usage example

from types_aiobotocore_privatenetworks.literals import NetworkFilterKeysType

def get_value() -> NetworkFilterKeysType:
    return "STATUS"
```

```python
# NetworkFilterKeysType definition

NetworkFilterKeysType = Literal[
    "STATUS",
]
```
## NetworkResourceDefinitionTypeType

```python
# NetworkResourceDefinitionTypeType usage example

from types_aiobotocore_privatenetworks.literals import NetworkResourceDefinitionTypeType

def get_value() -> NetworkResourceDefinitionTypeType:
    return "DEVICE_IDENTIFIER"
```

```python
# NetworkResourceDefinitionTypeType definition

NetworkResourceDefinitionTypeType = Literal[
    "DEVICE_IDENTIFIER",
    "RADIO_UNIT",
]
```
## NetworkResourceFilterKeysType

```python
# NetworkResourceFilterKeysType usage example

from types_aiobotocore_privatenetworks.literals import NetworkResourceFilterKeysType

def get_value() -> NetworkResourceFilterKeysType:
    return "ORDER"
```

```python
# NetworkResourceFilterKeysType definition

NetworkResourceFilterKeysType = Literal[
    "ORDER",
    "STATUS",
]
```
## NetworkResourceStatusType

```python
# NetworkResourceStatusType usage example

from types_aiobotocore_privatenetworks.literals import NetworkResourceStatusType

def get_value() -> NetworkResourceStatusType:
    return "AVAILABLE"
```

```python
# NetworkResourceStatusType definition

NetworkResourceStatusType = Literal[
    "AVAILABLE",
    "CREATING_SHIPPING_LABEL",
    "DELETED",
    "DELETING",
    "PENDING",
    "PENDING_RETURN",
    "PROVISIONED",
    "PROVISIONING",
    "SHIPPED",
]
```
## NetworkResourceTypeType

```python
# NetworkResourceTypeType usage example

from types_aiobotocore_privatenetworks.literals import NetworkResourceTypeType

def get_value() -> NetworkResourceTypeType:
    return "RADIO_UNIT"
```

```python
# NetworkResourceTypeType definition

NetworkResourceTypeType = Literal[
    "RADIO_UNIT",
]
```
## NetworkSiteFilterKeysType

```python
# NetworkSiteFilterKeysType usage example

from types_aiobotocore_privatenetworks.literals import NetworkSiteFilterKeysType

def get_value() -> NetworkSiteFilterKeysType:
    return "STATUS"
```

```python
# NetworkSiteFilterKeysType definition

NetworkSiteFilterKeysType = Literal[
    "STATUS",
]
```
## NetworkSiteStatusType

```python
# NetworkSiteStatusType usage example

from types_aiobotocore_privatenetworks.literals import NetworkSiteStatusType

def get_value() -> NetworkSiteStatusType:
    return "AVAILABLE"
```

```python
# NetworkSiteStatusType definition

NetworkSiteStatusType = Literal[
    "AVAILABLE",
    "CREATED",
    "DELETED",
    "DEPROVISIONING",
    "PROVISIONING",
]
```
## NetworkStatusType

```python
# NetworkStatusType usage example

from types_aiobotocore_privatenetworks.literals import NetworkStatusType

def get_value() -> NetworkStatusType:
    return "AVAILABLE"
```

```python
# NetworkStatusType definition

NetworkStatusType = Literal[
    "AVAILABLE",
    "CREATED",
    "DELETED",
    "DEPROVISIONING",
    "PROVISIONING",
]
```
## OrderFilterKeysType

```python
# OrderFilterKeysType usage example

from types_aiobotocore_privatenetworks.literals import OrderFilterKeysType

def get_value() -> OrderFilterKeysType:
    return "NETWORK_SITE"
```

```python
# OrderFilterKeysType definition

OrderFilterKeysType = Literal[
    "NETWORK_SITE",
    "STATUS",
]
```
## UpdateTypeType

```python
# UpdateTypeType usage example

from types_aiobotocore_privatenetworks.literals import UpdateTypeType

def get_value() -> UpdateTypeType:
    return "COMMITMENT"
```

```python
# UpdateTypeType definition

UpdateTypeType = Literal[
    "COMMITMENT",
    "REPLACE",
    "RETURN",
]
```
## Private5GServiceName

```python
# Private5GServiceName usage example

from types_aiobotocore_privatenetworks.literals import Private5GServiceName

def get_value() -> Private5GServiceName:
    return "privatenetworks"
```

```python
# Private5GServiceName definition

Private5GServiceName = Literal[
    "privatenetworks",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_privatenetworks.literals import ServiceName

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

from types_aiobotocore_privatenetworks.literals import ResourceServiceName

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

from types_aiobotocore_privatenetworks.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_device_identifiers"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_device_identifiers",
    "list_network_resources",
    "list_network_sites",
    "list_networks",
    "list_orders",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_privatenetworks.literals import RegionName

def get_value() -> RegionName:
    return "us-east-1"
```

```python
# RegionName definition

RegionName = Literal[
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
