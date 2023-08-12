# Literals

> [Index](../README.md) > [VPCLattice](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## AuthPolicyStateType

```python
# AuthPolicyStateType usage example

from types_aiobotocore_vpc_lattice.literals import AuthPolicyStateType

def get_value() -> AuthPolicyStateType:
    return "Active"
```

```python
# AuthPolicyStateType definition

AuthPolicyStateType = Literal[
    "Active",
    "Inactive",
]
```
## AuthTypeType

```python
# AuthTypeType usage example

from types_aiobotocore_vpc_lattice.literals import AuthTypeType

def get_value() -> AuthTypeType:
    return "AWS_IAM"
```

```python
# AuthTypeType definition

AuthTypeType = Literal[
    "AWS_IAM",
    "NONE",
]
```
## HealthCheckProtocolVersionType

```python
# HealthCheckProtocolVersionType usage example

from types_aiobotocore_vpc_lattice.literals import HealthCheckProtocolVersionType

def get_value() -> HealthCheckProtocolVersionType:
    return "HTTP1"
```

```python
# HealthCheckProtocolVersionType definition

HealthCheckProtocolVersionType = Literal[
    "HTTP1",
    "HTTP2",
]
```
## IpAddressTypeType

```python
# IpAddressTypeType usage example

from types_aiobotocore_vpc_lattice.literals import IpAddressTypeType

def get_value() -> IpAddressTypeType:
    return "IPV4"
```

```python
# IpAddressTypeType definition

IpAddressTypeType = Literal[
    "IPV4",
    "IPV6",
]
```
## ListAccessLogSubscriptionsPaginatorName

```python
# ListAccessLogSubscriptionsPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListAccessLogSubscriptionsPaginatorName

def get_value() -> ListAccessLogSubscriptionsPaginatorName:
    return "list_access_log_subscriptions"
```

```python
# ListAccessLogSubscriptionsPaginatorName definition

ListAccessLogSubscriptionsPaginatorName = Literal[
    "list_access_log_subscriptions",
]
```
## ListListenersPaginatorName

```python
# ListListenersPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListListenersPaginatorName

def get_value() -> ListListenersPaginatorName:
    return "list_listeners"
```

```python
# ListListenersPaginatorName definition

ListListenersPaginatorName = Literal[
    "list_listeners",
]
```
## ListRulesPaginatorName

```python
# ListRulesPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListRulesPaginatorName

def get_value() -> ListRulesPaginatorName:
    return "list_rules"
```

```python
# ListRulesPaginatorName definition

ListRulesPaginatorName = Literal[
    "list_rules",
]
```
## ListServiceNetworkServiceAssociationsPaginatorName

```python
# ListServiceNetworkServiceAssociationsPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListServiceNetworkServiceAssociationsPaginatorName

def get_value() -> ListServiceNetworkServiceAssociationsPaginatorName:
    return "list_service_network_service_associations"
```

```python
# ListServiceNetworkServiceAssociationsPaginatorName definition

ListServiceNetworkServiceAssociationsPaginatorName = Literal[
    "list_service_network_service_associations",
]
```
## ListServiceNetworkVpcAssociationsPaginatorName

```python
# ListServiceNetworkVpcAssociationsPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListServiceNetworkVpcAssociationsPaginatorName

def get_value() -> ListServiceNetworkVpcAssociationsPaginatorName:
    return "list_service_network_vpc_associations"
```

```python
# ListServiceNetworkVpcAssociationsPaginatorName definition

ListServiceNetworkVpcAssociationsPaginatorName = Literal[
    "list_service_network_vpc_associations",
]
```
## ListServiceNetworksPaginatorName

```python
# ListServiceNetworksPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListServiceNetworksPaginatorName

def get_value() -> ListServiceNetworksPaginatorName:
    return "list_service_networks"
```

```python
# ListServiceNetworksPaginatorName definition

ListServiceNetworksPaginatorName = Literal[
    "list_service_networks",
]
```
## ListServicesPaginatorName

```python
# ListServicesPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListServicesPaginatorName

def get_value() -> ListServicesPaginatorName:
    return "list_services"
```

```python
# ListServicesPaginatorName definition

ListServicesPaginatorName = Literal[
    "list_services",
]
```
## ListTargetGroupsPaginatorName

```python
# ListTargetGroupsPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListTargetGroupsPaginatorName

def get_value() -> ListTargetGroupsPaginatorName:
    return "list_target_groups"
```

```python
# ListTargetGroupsPaginatorName definition

ListTargetGroupsPaginatorName = Literal[
    "list_target_groups",
]
```
## ListTargetsPaginatorName

```python
# ListTargetsPaginatorName usage example

from types_aiobotocore_vpc_lattice.literals import ListTargetsPaginatorName

def get_value() -> ListTargetsPaginatorName:
    return "list_targets"
```

```python
# ListTargetsPaginatorName definition

ListTargetsPaginatorName = Literal[
    "list_targets",
]
```
## ListenerProtocolType

```python
# ListenerProtocolType usage example

from types_aiobotocore_vpc_lattice.literals import ListenerProtocolType

def get_value() -> ListenerProtocolType:
    return "HTTP"
```

```python
# ListenerProtocolType definition

ListenerProtocolType = Literal[
    "HTTP",
    "HTTPS",
]
```
## ServiceNetworkServiceAssociationStatusType

```python
# ServiceNetworkServiceAssociationStatusType usage example

from types_aiobotocore_vpc_lattice.literals import ServiceNetworkServiceAssociationStatusType

def get_value() -> ServiceNetworkServiceAssociationStatusType:
    return "ACTIVE"
```

```python
# ServiceNetworkServiceAssociationStatusType definition

ServiceNetworkServiceAssociationStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
]
```
## ServiceNetworkVpcAssociationStatusType

```python
# ServiceNetworkVpcAssociationStatusType usage example

from types_aiobotocore_vpc_lattice.literals import ServiceNetworkVpcAssociationStatusType

def get_value() -> ServiceNetworkVpcAssociationStatusType:
    return "ACTIVE"
```

```python
# ServiceNetworkVpcAssociationStatusType definition

ServiceNetworkVpcAssociationStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## ServiceStatusType

```python
# ServiceStatusType usage example

from types_aiobotocore_vpc_lattice.literals import ServiceStatusType

def get_value() -> ServiceStatusType:
    return "ACTIVE"
```

```python
# ServiceStatusType definition

ServiceStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
]
```
## TargetGroupProtocolType

```python
# TargetGroupProtocolType usage example

from types_aiobotocore_vpc_lattice.literals import TargetGroupProtocolType

def get_value() -> TargetGroupProtocolType:
    return "HTTP"
```

```python
# TargetGroupProtocolType definition

TargetGroupProtocolType = Literal[
    "HTTP",
    "HTTPS",
]
```
## TargetGroupProtocolVersionType

```python
# TargetGroupProtocolVersionType usage example

from types_aiobotocore_vpc_lattice.literals import TargetGroupProtocolVersionType

def get_value() -> TargetGroupProtocolVersionType:
    return "GRPC"
```

```python
# TargetGroupProtocolVersionType definition

TargetGroupProtocolVersionType = Literal[
    "GRPC",
    "HTTP1",
    "HTTP2",
]
```
## TargetGroupStatusType

```python
# TargetGroupStatusType usage example

from types_aiobotocore_vpc_lattice.literals import TargetGroupStatusType

def get_value() -> TargetGroupStatusType:
    return "ACTIVE"
```

```python
# TargetGroupStatusType definition

TargetGroupStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
]
```
## TargetGroupTypeType

```python
# TargetGroupTypeType usage example

from types_aiobotocore_vpc_lattice.literals import TargetGroupTypeType

def get_value() -> TargetGroupTypeType:
    return "ALB"
```

```python
# TargetGroupTypeType definition

TargetGroupTypeType = Literal[
    "ALB",
    "INSTANCE",
    "IP",
    "LAMBDA",
]
```
## TargetStatusType

```python
# TargetStatusType usage example

from types_aiobotocore_vpc_lattice.literals import TargetStatusType

def get_value() -> TargetStatusType:
    return "DRAINING"
```

```python
# TargetStatusType definition

TargetStatusType = Literal[
    "DRAINING",
    "HEALTHY",
    "INITIAL",
    "UNAVAILABLE",
    "UNHEALTHY",
    "UNUSED",
]
```
## VPCLatticeServiceName

```python
# VPCLatticeServiceName usage example

from types_aiobotocore_vpc_lattice.literals import VPCLatticeServiceName

def get_value() -> VPCLatticeServiceName:
    return "vpc-lattice"
```

```python
# VPCLatticeServiceName definition

VPCLatticeServiceName = Literal[
    "vpc-lattice",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_vpc_lattice.literals import ServiceName

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

from types_aiobotocore_vpc_lattice.literals import ResourceServiceName

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

from types_aiobotocore_vpc_lattice.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_access_log_subscriptions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_access_log_subscriptions",
    "list_listeners",
    "list_rules",
    "list_service_network_service_associations",
    "list_service_network_vpc_associations",
    "list_service_networks",
    "list_services",
    "list_target_groups",
    "list_targets",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_vpc_lattice.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
