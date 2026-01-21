# Literals

> [Index](../README.md) > [Odb](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb)
    type annotations stubs module [types-aiobotocore-odb](https://pypi.org/project/types-aiobotocore-odb/).

## AccessType

```python
# AccessType usage example
from types_aiobotocore_odb.literals import AccessType

def get_value() -> AccessType:
    return "DISABLED"
```

```python
# AccessType definition
AccessType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ComputeModelType

```python
# ComputeModelType usage example
from types_aiobotocore_odb.literals import ComputeModelType

def get_value() -> ComputeModelType:
    return "ECPU"
```

```python
# ComputeModelType definition
ComputeModelType = Literal[
    "ECPU",
    "OCPU",
]
```
## DayOfWeekNameType

```python
# DayOfWeekNameType usage example
from types_aiobotocore_odb.literals import DayOfWeekNameType

def get_value() -> DayOfWeekNameType:
    return "FRIDAY"
```

```python
# DayOfWeekNameType definition
DayOfWeekNameType = Literal[
    "FRIDAY",
    "MONDAY",
    "SATURDAY",
    "SUNDAY",
    "THURSDAY",
    "TUESDAY",
    "WEDNESDAY",
]
```
## DbNodeMaintenanceTypeType

```python
# DbNodeMaintenanceTypeType usage example
from types_aiobotocore_odb.literals import DbNodeMaintenanceTypeType

def get_value() -> DbNodeMaintenanceTypeType:
    return "VMDB_REBOOT_MIGRATION"
```

```python
# DbNodeMaintenanceTypeType definition
DbNodeMaintenanceTypeType = Literal[
    "VMDB_REBOOT_MIGRATION",
]
```
## DbNodeResourceStatusType

```python
# DbNodeResourceStatusType usage example
from types_aiobotocore_odb.literals import DbNodeResourceStatusType

def get_value() -> DbNodeResourceStatusType:
    return "AVAILABLE"
```

```python
# DbNodeResourceStatusType definition
DbNodeResourceStatusType = Literal[
    "AVAILABLE",
    "FAILED",
    "PROVISIONING",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "TERMINATED",
    "TERMINATING",
    "UPDATING",
]
```
## DbServerPatchingStatusType

```python
# DbServerPatchingStatusType usage example
from types_aiobotocore_odb.literals import DbServerPatchingStatusType

def get_value() -> DbServerPatchingStatusType:
    return "COMPLETE"
```

```python
# DbServerPatchingStatusType definition
DbServerPatchingStatusType = Literal[
    "COMPLETE",
    "FAILED",
    "MAINTENANCE_IN_PROGRESS",
    "SCHEDULED",
]
```
## DiskRedundancyType

```python
# DiskRedundancyType usage example
from types_aiobotocore_odb.literals import DiskRedundancyType

def get_value() -> DiskRedundancyType:
    return "HIGH"
```

```python
# DiskRedundancyType definition
DiskRedundancyType = Literal[
    "HIGH",
    "NORMAL",
]
```
## IamRoleStatusType

```python
# IamRoleStatusType usage example
from types_aiobotocore_odb.literals import IamRoleStatusType

def get_value() -> IamRoleStatusType:
    return "ASSOCIATING"
```

```python
# IamRoleStatusType definition
IamRoleStatusType = Literal[
    "ASSOCIATING",
    "CONNECTED",
    "DISASSOCIATING",
    "DISCONNECTED",
    "FAILED",
    "PARTIALLY_CONNECTED",
    "UNKNOWN",
]
```
## IormLifecycleStateType

```python
# IormLifecycleStateType usage example
from types_aiobotocore_odb.literals import IormLifecycleStateType

def get_value() -> IormLifecycleStateType:
    return "BOOTSTRAPPING"
```

```python
# IormLifecycleStateType definition
IormLifecycleStateType = Literal[
    "BOOTSTRAPPING",
    "DISABLED",
    "ENABLED",
    "FAILED",
    "UPDATING",
]
```
## LicenseModelType

```python
# LicenseModelType usage example
from types_aiobotocore_odb.literals import LicenseModelType

def get_value() -> LicenseModelType:
    return "BRING_YOUR_OWN_LICENSE"
```

```python
# LicenseModelType definition
LicenseModelType = Literal[
    "BRING_YOUR_OWN_LICENSE",
    "LICENSE_INCLUDED",
]
```
## ListAutonomousVirtualMachinesPaginatorName

```python
# ListAutonomousVirtualMachinesPaginatorName usage example
from types_aiobotocore_odb.literals import ListAutonomousVirtualMachinesPaginatorName

def get_value() -> ListAutonomousVirtualMachinesPaginatorName:
    return "list_autonomous_virtual_machines"
```

```python
# ListAutonomousVirtualMachinesPaginatorName definition
ListAutonomousVirtualMachinesPaginatorName = Literal[
    "list_autonomous_virtual_machines",
]
```
## ListCloudAutonomousVmClustersPaginatorName

```python
# ListCloudAutonomousVmClustersPaginatorName usage example
from types_aiobotocore_odb.literals import ListCloudAutonomousVmClustersPaginatorName

def get_value() -> ListCloudAutonomousVmClustersPaginatorName:
    return "list_cloud_autonomous_vm_clusters"
```

```python
# ListCloudAutonomousVmClustersPaginatorName definition
ListCloudAutonomousVmClustersPaginatorName = Literal[
    "list_cloud_autonomous_vm_clusters",
]
```
## ListCloudExadataInfrastructuresPaginatorName

```python
# ListCloudExadataInfrastructuresPaginatorName usage example
from types_aiobotocore_odb.literals import ListCloudExadataInfrastructuresPaginatorName

def get_value() -> ListCloudExadataInfrastructuresPaginatorName:
    return "list_cloud_exadata_infrastructures"
```

```python
# ListCloudExadataInfrastructuresPaginatorName definition
ListCloudExadataInfrastructuresPaginatorName = Literal[
    "list_cloud_exadata_infrastructures",
]
```
## ListCloudVmClustersPaginatorName

```python
# ListCloudVmClustersPaginatorName usage example
from types_aiobotocore_odb.literals import ListCloudVmClustersPaginatorName

def get_value() -> ListCloudVmClustersPaginatorName:
    return "list_cloud_vm_clusters"
```

```python
# ListCloudVmClustersPaginatorName definition
ListCloudVmClustersPaginatorName = Literal[
    "list_cloud_vm_clusters",
]
```
## ListDbNodesPaginatorName

```python
# ListDbNodesPaginatorName usage example
from types_aiobotocore_odb.literals import ListDbNodesPaginatorName

def get_value() -> ListDbNodesPaginatorName:
    return "list_db_nodes"
```

```python
# ListDbNodesPaginatorName definition
ListDbNodesPaginatorName = Literal[
    "list_db_nodes",
]
```
## ListDbServersPaginatorName

```python
# ListDbServersPaginatorName usage example
from types_aiobotocore_odb.literals import ListDbServersPaginatorName

def get_value() -> ListDbServersPaginatorName:
    return "list_db_servers"
```

```python
# ListDbServersPaginatorName definition
ListDbServersPaginatorName = Literal[
    "list_db_servers",
]
```
## ListDbSystemShapesPaginatorName

```python
# ListDbSystemShapesPaginatorName usage example
from types_aiobotocore_odb.literals import ListDbSystemShapesPaginatorName

def get_value() -> ListDbSystemShapesPaginatorName:
    return "list_db_system_shapes"
```

```python
# ListDbSystemShapesPaginatorName definition
ListDbSystemShapesPaginatorName = Literal[
    "list_db_system_shapes",
]
```
## ListGiVersionsPaginatorName

```python
# ListGiVersionsPaginatorName usage example
from types_aiobotocore_odb.literals import ListGiVersionsPaginatorName

def get_value() -> ListGiVersionsPaginatorName:
    return "list_gi_versions"
```

```python
# ListGiVersionsPaginatorName definition
ListGiVersionsPaginatorName = Literal[
    "list_gi_versions",
]
```
## ListOdbNetworksPaginatorName

```python
# ListOdbNetworksPaginatorName usage example
from types_aiobotocore_odb.literals import ListOdbNetworksPaginatorName

def get_value() -> ListOdbNetworksPaginatorName:
    return "list_odb_networks"
```

```python
# ListOdbNetworksPaginatorName definition
ListOdbNetworksPaginatorName = Literal[
    "list_odb_networks",
]
```
## ListOdbPeeringConnectionsPaginatorName

```python
# ListOdbPeeringConnectionsPaginatorName usage example
from types_aiobotocore_odb.literals import ListOdbPeeringConnectionsPaginatorName

def get_value() -> ListOdbPeeringConnectionsPaginatorName:
    return "list_odb_peering_connections"
```

```python
# ListOdbPeeringConnectionsPaginatorName definition
ListOdbPeeringConnectionsPaginatorName = Literal[
    "list_odb_peering_connections",
]
```
## ListSystemVersionsPaginatorName

```python
# ListSystemVersionsPaginatorName usage example
from types_aiobotocore_odb.literals import ListSystemVersionsPaginatorName

def get_value() -> ListSystemVersionsPaginatorName:
    return "list_system_versions"
```

```python
# ListSystemVersionsPaginatorName definition
ListSystemVersionsPaginatorName = Literal[
    "list_system_versions",
]
```
## ManagedResourceStatusType

```python
# ManagedResourceStatusType usage example
from types_aiobotocore_odb.literals import ManagedResourceStatusType

def get_value() -> ManagedResourceStatusType:
    return "DISABLED"
```

```python
# ManagedResourceStatusType definition
ManagedResourceStatusType = Literal[
    "DISABLED",
    "DISABLING",
    "ENABLED",
    "ENABLING",
]
```
## MonthNameType

```python
# MonthNameType usage example
from types_aiobotocore_odb.literals import MonthNameType

def get_value() -> MonthNameType:
    return "APRIL"
```

```python
# MonthNameType definition
MonthNameType = Literal[
    "APRIL",
    "AUGUST",
    "DECEMBER",
    "FEBRUARY",
    "JANUARY",
    "JULY",
    "JUNE",
    "MARCH",
    "MAY",
    "NOVEMBER",
    "OCTOBER",
    "SEPTEMBER",
]
```
## ObjectiveType

```python
# ObjectiveType usage example
from types_aiobotocore_odb.literals import ObjectiveType

def get_value() -> ObjectiveType:
    return "AUTO"
```

```python
# ObjectiveType definition
ObjectiveType = Literal[
    "AUTO",
    "BALANCED",
    "BASIC",
    "HIGH_THROUGHPUT",
    "LOW_LATENCY",
]
```
## OciOnboardingStatusType

```python
# OciOnboardingStatusType usage example
from types_aiobotocore_odb.literals import OciOnboardingStatusType

def get_value() -> OciOnboardingStatusType:
    return "ACTIVATING"
```

```python
# OciOnboardingStatusType definition
OciOnboardingStatusType = Literal[
    "ACTIVATING",
    "ACTIVE",
    "ACTIVE_IN_HOME_REGION",
    "ACTIVE_LIMITED",
    "CANCELED",
    "FAILED",
    "NOT_STARTED",
    "PENDING_CUSTOMER_ACTION",
    "PENDING_INITIALIZATION",
    "PENDING_LINK_GENERATION",
    "PUBLIC_OFFER_UNSUPPORTED",
    "SUSPENDED",
]
```
## PatchingModeTypeType

```python
# PatchingModeTypeType usage example
from types_aiobotocore_odb.literals import PatchingModeTypeType

def get_value() -> PatchingModeTypeType:
    return "NONROLLING"
```

```python
# PatchingModeTypeType definition
PatchingModeTypeType = Literal[
    "NONROLLING",
    "ROLLING",
]
```
## PreferenceTypeType

```python
# PreferenceTypeType usage example
from types_aiobotocore_odb.literals import PreferenceTypeType

def get_value() -> PreferenceTypeType:
    return "CUSTOM_PREFERENCE"
```

```python
# PreferenceTypeType definition
PreferenceTypeType = Literal[
    "CUSTOM_PREFERENCE",
    "NO_PREFERENCE",
]
```
## ResourceStatusType

```python
# ResourceStatusType usage example
from types_aiobotocore_odb.literals import ResourceStatusType

def get_value() -> ResourceStatusType:
    return "AVAILABLE"
```

```python
# ResourceStatusType definition
ResourceStatusType = Literal[
    "AVAILABLE",
    "FAILED",
    "MAINTENANCE_IN_PROGRESS",
    "PROVISIONING",
    "TERMINATED",
    "TERMINATING",
    "UPDATING",
]
```
## ShapeTypeType

```python
# ShapeTypeType usage example
from types_aiobotocore_odb.literals import ShapeTypeType

def get_value() -> ShapeTypeType:
    return "AMD"
```

```python
# ShapeTypeType definition
ShapeTypeType = Literal[
    "AMD",
    "AMPERE_FLEX_A1",
    "INTEL",
    "INTEL_FLEX_X9",
]
```
## SupportedAwsIntegrationType

```python
# SupportedAwsIntegrationType usage example
from types_aiobotocore_odb.literals import SupportedAwsIntegrationType

def get_value() -> SupportedAwsIntegrationType:
    return "KmsTde"
```

```python
# SupportedAwsIntegrationType definition
SupportedAwsIntegrationType = Literal[
    "KmsTde",
]
```
## VpcEndpointTypeType

```python
# VpcEndpointTypeType usage example
from types_aiobotocore_odb.literals import VpcEndpointTypeType

def get_value() -> VpcEndpointTypeType:
    return "SERVICENETWORK"
```

```python
# VpcEndpointTypeType definition
VpcEndpointTypeType = Literal[
    "SERVICENETWORK",
]
```
## OdbServiceName

```python
# OdbServiceName usage example
from types_aiobotocore_odb.literals import OdbServiceName

def get_value() -> OdbServiceName:
    return "odb"
```

```python
# OdbServiceName definition
OdbServiceName = Literal[
    "odb",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_odb.literals import ServiceName

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
from types_aiobotocore_odb.literals import ResourceServiceName

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
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_odb.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_autonomous_virtual_machines"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_autonomous_virtual_machines",
    "list_cloud_autonomous_vm_clusters",
    "list_cloud_exadata_infrastructures",
    "list_cloud_vm_clusters",
    "list_db_nodes",
    "list_db_servers",
    "list_db_system_shapes",
    "list_gi_versions",
    "list_odb_networks",
    "list_odb_peering_connections",
    "list_system_versions",
]
```
