# Literals

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

## AcceleratorStatusType

```python
# AcceleratorStatusType usage example

from types_aiobotocore_globalaccelerator.literals import AcceleratorStatusType

def get_value() -> AcceleratorStatusType:
    return "DEPLOYED"
```

```python
# AcceleratorStatusType definition

AcceleratorStatusType = Literal[
    "DEPLOYED",
    "IN_PROGRESS",
]
```
## ByoipCidrStateType

```python
# ByoipCidrStateType usage example

from types_aiobotocore_globalaccelerator.literals import ByoipCidrStateType

def get_value() -> ByoipCidrStateType:
    return "ADVERTISING"
```

```python
# ByoipCidrStateType definition

ByoipCidrStateType = Literal[
    "ADVERTISING",
    "DEPROVISIONED",
    "FAILED_ADVERTISING",
    "FAILED_DEPROVISION",
    "FAILED_PROVISION",
    "FAILED_WITHDRAW",
    "PENDING_ADVERTISING",
    "PENDING_DEPROVISIONING",
    "PENDING_PROVISIONING",
    "PENDING_WITHDRAWING",
    "READY",
]
```
## ClientAffinityType

```python
# ClientAffinityType usage example

from types_aiobotocore_globalaccelerator.literals import ClientAffinityType

def get_value() -> ClientAffinityType:
    return "NONE"
```

```python
# ClientAffinityType definition

ClientAffinityType = Literal[
    "NONE",
    "SOURCE_IP",
]
```
## CustomRoutingAcceleratorStatusType

```python
# CustomRoutingAcceleratorStatusType usage example

from types_aiobotocore_globalaccelerator.literals import CustomRoutingAcceleratorStatusType

def get_value() -> CustomRoutingAcceleratorStatusType:
    return "DEPLOYED"
```

```python
# CustomRoutingAcceleratorStatusType definition

CustomRoutingAcceleratorStatusType = Literal[
    "DEPLOYED",
    "IN_PROGRESS",
]
```
## CustomRoutingDestinationTrafficStateType

```python
# CustomRoutingDestinationTrafficStateType usage example

from types_aiobotocore_globalaccelerator.literals import CustomRoutingDestinationTrafficStateType

def get_value() -> CustomRoutingDestinationTrafficStateType:
    return "ALLOW"
```

```python
# CustomRoutingDestinationTrafficStateType definition

CustomRoutingDestinationTrafficStateType = Literal[
    "ALLOW",
    "DENY",
]
```
## CustomRoutingProtocolType

```python
# CustomRoutingProtocolType usage example

from types_aiobotocore_globalaccelerator.literals import CustomRoutingProtocolType

def get_value() -> CustomRoutingProtocolType:
    return "TCP"
```

```python
# CustomRoutingProtocolType definition

CustomRoutingProtocolType = Literal[
    "TCP",
    "UDP",
]
```
## HealthCheckProtocolType

```python
# HealthCheckProtocolType usage example

from types_aiobotocore_globalaccelerator.literals import HealthCheckProtocolType

def get_value() -> HealthCheckProtocolType:
    return "HTTP"
```

```python
# HealthCheckProtocolType definition

HealthCheckProtocolType = Literal[
    "HTTP",
    "HTTPS",
    "TCP",
]
```
## HealthStateType

```python
# HealthStateType usage example

from types_aiobotocore_globalaccelerator.literals import HealthStateType

def get_value() -> HealthStateType:
    return "HEALTHY"
```

```python
# HealthStateType definition

HealthStateType = Literal[
    "HEALTHY",
    "INITIAL",
    "UNHEALTHY",
]
```
## IpAddressFamilyType

```python
# IpAddressFamilyType usage example

from types_aiobotocore_globalaccelerator.literals import IpAddressFamilyType

def get_value() -> IpAddressFamilyType:
    return "IPv4"
```

```python
# IpAddressFamilyType definition

IpAddressFamilyType = Literal[
    "IPv4",
    "IPv6",
]
```
## IpAddressTypeType

```python
# IpAddressTypeType usage example

from types_aiobotocore_globalaccelerator.literals import IpAddressTypeType

def get_value() -> IpAddressTypeType:
    return "DUAL_STACK"
```

```python
# IpAddressTypeType definition

IpAddressTypeType = Literal[
    "DUAL_STACK",
    "IPV4",
]
```
## ListAcceleratorsPaginatorName

```python
# ListAcceleratorsPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListAcceleratorsPaginatorName

def get_value() -> ListAcceleratorsPaginatorName:
    return "list_accelerators"
```

```python
# ListAcceleratorsPaginatorName definition

ListAcceleratorsPaginatorName = Literal[
    "list_accelerators",
]
```
## ListByoipCidrsPaginatorName

```python
# ListByoipCidrsPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListByoipCidrsPaginatorName

def get_value() -> ListByoipCidrsPaginatorName:
    return "list_byoip_cidrs"
```

```python
# ListByoipCidrsPaginatorName definition

ListByoipCidrsPaginatorName = Literal[
    "list_byoip_cidrs",
]
```
## ListCustomRoutingAcceleratorsPaginatorName

```python
# ListCustomRoutingAcceleratorsPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListCustomRoutingAcceleratorsPaginatorName

def get_value() -> ListCustomRoutingAcceleratorsPaginatorName:
    return "list_custom_routing_accelerators"
```

```python
# ListCustomRoutingAcceleratorsPaginatorName definition

ListCustomRoutingAcceleratorsPaginatorName = Literal[
    "list_custom_routing_accelerators",
]
```
## ListCustomRoutingListenersPaginatorName

```python
# ListCustomRoutingListenersPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListCustomRoutingListenersPaginatorName

def get_value() -> ListCustomRoutingListenersPaginatorName:
    return "list_custom_routing_listeners"
```

```python
# ListCustomRoutingListenersPaginatorName definition

ListCustomRoutingListenersPaginatorName = Literal[
    "list_custom_routing_listeners",
]
```
## ListCustomRoutingPortMappingsByDestinationPaginatorName

```python
# ListCustomRoutingPortMappingsByDestinationPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListCustomRoutingPortMappingsByDestinationPaginatorName

def get_value() -> ListCustomRoutingPortMappingsByDestinationPaginatorName:
    return "list_custom_routing_port_mappings_by_destination"
```

```python
# ListCustomRoutingPortMappingsByDestinationPaginatorName definition

ListCustomRoutingPortMappingsByDestinationPaginatorName = Literal[
    "list_custom_routing_port_mappings_by_destination",
]
```
## ListCustomRoutingPortMappingsPaginatorName

```python
# ListCustomRoutingPortMappingsPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListCustomRoutingPortMappingsPaginatorName

def get_value() -> ListCustomRoutingPortMappingsPaginatorName:
    return "list_custom_routing_port_mappings"
```

```python
# ListCustomRoutingPortMappingsPaginatorName definition

ListCustomRoutingPortMappingsPaginatorName = Literal[
    "list_custom_routing_port_mappings",
]
```
## ListEndpointGroupsPaginatorName

```python
# ListEndpointGroupsPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListEndpointGroupsPaginatorName

def get_value() -> ListEndpointGroupsPaginatorName:
    return "list_endpoint_groups"
```

```python
# ListEndpointGroupsPaginatorName definition

ListEndpointGroupsPaginatorName = Literal[
    "list_endpoint_groups",
]
```
## ListListenersPaginatorName

```python
# ListListenersPaginatorName usage example

from types_aiobotocore_globalaccelerator.literals import ListListenersPaginatorName

def get_value() -> ListListenersPaginatorName:
    return "list_listeners"
```

```python
# ListListenersPaginatorName definition

ListListenersPaginatorName = Literal[
    "list_listeners",
]
```
## ProtocolType

```python
# ProtocolType usage example

from types_aiobotocore_globalaccelerator.literals import ProtocolType

def get_value() -> ProtocolType:
    return "TCP"
```

```python
# ProtocolType definition

ProtocolType = Literal[
    "TCP",
    "UDP",
]
```
## GlobalAcceleratorServiceName

```python
# GlobalAcceleratorServiceName usage example

from types_aiobotocore_globalaccelerator.literals import GlobalAcceleratorServiceName

def get_value() -> GlobalAcceleratorServiceName:
    return "globalaccelerator"
```

```python
# GlobalAcceleratorServiceName definition

GlobalAcceleratorServiceName = Literal[
    "globalaccelerator",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_globalaccelerator.literals import ServiceName

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

from types_aiobotocore_globalaccelerator.literals import ResourceServiceName

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

from types_aiobotocore_globalaccelerator.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_accelerators"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_accelerators",
    "list_byoip_cidrs",
    "list_custom_routing_accelerators",
    "list_custom_routing_listeners",
    "list_custom_routing_port_mappings",
    "list_custom_routing_port_mappings_by_destination",
    "list_endpoint_groups",
    "list_listeners",
]
```
