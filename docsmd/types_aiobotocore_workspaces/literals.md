# Literals

> [Index](../README.md) > [WorkSpaces](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## AccessPropertyValueType

```python
# AccessPropertyValueType usage example

from types_aiobotocore_workspaces.literals import AccessPropertyValueType

def get_value() -> AccessPropertyValueType:
    return "ALLOW"
```

```python
# AccessPropertyValueType definition

AccessPropertyValueType = Literal[
    "ALLOW",
    "DENY",
]
```
## ApplicationType

```python
# ApplicationType usage example

from types_aiobotocore_workspaces.literals import ApplicationType

def get_value() -> ApplicationType:
    return "Microsoft_Office_2016"
```

```python
# ApplicationType definition

ApplicationType = Literal[
    "Microsoft_Office_2016",
    "Microsoft_Office_2019",
]
```
## AssociationStatusType

```python
# AssociationStatusType usage example

from types_aiobotocore_workspaces.literals import AssociationStatusType

def get_value() -> AssociationStatusType:
    return "ASSOCIATED_WITH_OWNER_ACCOUNT"
```

```python
# AssociationStatusType definition

AssociationStatusType = Literal[
    "ASSOCIATED_WITH_OWNER_ACCOUNT",
    "ASSOCIATED_WITH_SHARED_ACCOUNT",
    "NOT_ASSOCIATED",
    "PENDING_ASSOCIATION",
    "PENDING_DISASSOCIATION",
]
```
## BundleTypeType

```python
# BundleTypeType usage example

from types_aiobotocore_workspaces.literals import BundleTypeType

def get_value() -> BundleTypeType:
    return "REGULAR"
```

```python
# BundleTypeType definition

BundleTypeType = Literal[
    "REGULAR",
    "STANDBY",
]
```
## CertificateBasedAuthStatusEnumType

```python
# CertificateBasedAuthStatusEnumType usage example

from types_aiobotocore_workspaces.literals import CertificateBasedAuthStatusEnumType

def get_value() -> CertificateBasedAuthStatusEnumType:
    return "DISABLED"
```

```python
# CertificateBasedAuthStatusEnumType definition

CertificateBasedAuthStatusEnumType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ClientDeviceTypeType

```python
# ClientDeviceTypeType usage example

from types_aiobotocore_workspaces.literals import ClientDeviceTypeType

def get_value() -> ClientDeviceTypeType:
    return "DeviceTypeAndroid"
```

```python
# ClientDeviceTypeType definition

ClientDeviceTypeType = Literal[
    "DeviceTypeAndroid",
    "DeviceTypeIos",
    "DeviceTypeLinux",
    "DeviceTypeOsx",
    "DeviceTypeWeb",
    "DeviceTypeWindows",
]
```
## ComputeType

```python
# ComputeType usage example

from types_aiobotocore_workspaces.literals import ComputeType

def get_value() -> ComputeType:
    return "GRAPHICS"
```

```python
# ComputeType definition

ComputeType = Literal[
    "GRAPHICS",
    "GRAPHICS_G4DN",
    "GRAPHICSPRO",
    "GRAPHICSPRO_G4DN",
    "PERFORMANCE",
    "POWER",
    "POWERPRO",
    "STANDARD",
    "VALUE",
]
```
## ConnectionAliasStateType

```python
# ConnectionAliasStateType usage example

from types_aiobotocore_workspaces.literals import ConnectionAliasStateType

def get_value() -> ConnectionAliasStateType:
    return "CREATED"
```

```python
# ConnectionAliasStateType definition

ConnectionAliasStateType = Literal[
    "CREATED",
    "CREATING",
    "DELETING",
]
```
## ConnectionStateType

```python
# ConnectionStateType usage example

from types_aiobotocore_workspaces.literals import ConnectionStateType

def get_value() -> ConnectionStateType:
    return "CONNECTED"
```

```python
# ConnectionStateType definition

ConnectionStateType = Literal[
    "CONNECTED",
    "DISCONNECTED",
    "UNKNOWN",
]
```
## DedicatedTenancyModificationStateEnumType

```python
# DedicatedTenancyModificationStateEnumType usage example

from types_aiobotocore_workspaces.literals import DedicatedTenancyModificationStateEnumType

def get_value() -> DedicatedTenancyModificationStateEnumType:
    return "COMPLETED"
```

```python
# DedicatedTenancyModificationStateEnumType definition

DedicatedTenancyModificationStateEnumType = Literal[
    "COMPLETED",
    "FAILED",
    "PENDING",
]
```
## DedicatedTenancySupportEnumType

```python
# DedicatedTenancySupportEnumType usage example

from types_aiobotocore_workspaces.literals import DedicatedTenancySupportEnumType

def get_value() -> DedicatedTenancySupportEnumType:
    return "ENABLED"
```

```python
# DedicatedTenancySupportEnumType definition

DedicatedTenancySupportEnumType = Literal[
    "ENABLED",
]
```
## DedicatedTenancySupportResultEnumType

```python
# DedicatedTenancySupportResultEnumType usage example

from types_aiobotocore_workspaces.literals import DedicatedTenancySupportResultEnumType

def get_value() -> DedicatedTenancySupportResultEnumType:
    return "DISABLED"
```

```python
# DedicatedTenancySupportResultEnumType definition

DedicatedTenancySupportResultEnumType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## DeletableCertificateBasedAuthPropertyType

```python
# DeletableCertificateBasedAuthPropertyType usage example

from types_aiobotocore_workspaces.literals import DeletableCertificateBasedAuthPropertyType

def get_value() -> DeletableCertificateBasedAuthPropertyType:
    return "CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"
```

```python
# DeletableCertificateBasedAuthPropertyType definition

DeletableCertificateBasedAuthPropertyType = Literal[
    "CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN",
]
```
## DeletableSamlPropertyType

```python
# DeletableSamlPropertyType usage example

from types_aiobotocore_workspaces.literals import DeletableSamlPropertyType

def get_value() -> DeletableSamlPropertyType:
    return "SAML_PROPERTIES_RELAY_STATE_PARAMETER_NAME"
```

```python
# DeletableSamlPropertyType definition

DeletableSamlPropertyType = Literal[
    "SAML_PROPERTIES_RELAY_STATE_PARAMETER_NAME",
    "SAML_PROPERTIES_USER_ACCESS_URL",
]
```
## DescribeAccountModificationsPaginatorName

```python
# DescribeAccountModificationsPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeAccountModificationsPaginatorName

def get_value() -> DescribeAccountModificationsPaginatorName:
    return "describe_account_modifications"
```

```python
# DescribeAccountModificationsPaginatorName definition

DescribeAccountModificationsPaginatorName = Literal[
    "describe_account_modifications",
]
```
## DescribeIpGroupsPaginatorName

```python
# DescribeIpGroupsPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeIpGroupsPaginatorName

def get_value() -> DescribeIpGroupsPaginatorName:
    return "describe_ip_groups"
```

```python
# DescribeIpGroupsPaginatorName definition

DescribeIpGroupsPaginatorName = Literal[
    "describe_ip_groups",
]
```
## DescribeWorkspaceBundlesPaginatorName

```python
# DescribeWorkspaceBundlesPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeWorkspaceBundlesPaginatorName

def get_value() -> DescribeWorkspaceBundlesPaginatorName:
    return "describe_workspace_bundles"
```

```python
# DescribeWorkspaceBundlesPaginatorName definition

DescribeWorkspaceBundlesPaginatorName = Literal[
    "describe_workspace_bundles",
]
```
## DescribeWorkspaceDirectoriesPaginatorName

```python
# DescribeWorkspaceDirectoriesPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeWorkspaceDirectoriesPaginatorName

def get_value() -> DescribeWorkspaceDirectoriesPaginatorName:
    return "describe_workspace_directories"
```

```python
# DescribeWorkspaceDirectoriesPaginatorName definition

DescribeWorkspaceDirectoriesPaginatorName = Literal[
    "describe_workspace_directories",
]
```
## DescribeWorkspaceImagesPaginatorName

```python
# DescribeWorkspaceImagesPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeWorkspaceImagesPaginatorName

def get_value() -> DescribeWorkspaceImagesPaginatorName:
    return "describe_workspace_images"
```

```python
# DescribeWorkspaceImagesPaginatorName definition

DescribeWorkspaceImagesPaginatorName = Literal[
    "describe_workspace_images",
]
```
## DescribeWorkspacesConnectionStatusPaginatorName

```python
# DescribeWorkspacesConnectionStatusPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeWorkspacesConnectionStatusPaginatorName

def get_value() -> DescribeWorkspacesConnectionStatusPaginatorName:
    return "describe_workspaces_connection_status"
```

```python
# DescribeWorkspacesConnectionStatusPaginatorName definition

DescribeWorkspacesConnectionStatusPaginatorName = Literal[
    "describe_workspaces_connection_status",
]
```
## DescribeWorkspacesPaginatorName

```python
# DescribeWorkspacesPaginatorName usage example

from types_aiobotocore_workspaces.literals import DescribeWorkspacesPaginatorName

def get_value() -> DescribeWorkspacesPaginatorName:
    return "describe_workspaces"
```

```python
# DescribeWorkspacesPaginatorName definition

DescribeWorkspacesPaginatorName = Literal[
    "describe_workspaces",
]
```
## ImageTypeType

```python
# ImageTypeType usage example

from types_aiobotocore_workspaces.literals import ImageTypeType

def get_value() -> ImageTypeType:
    return "OWNED"
```

```python
# ImageTypeType definition

ImageTypeType = Literal[
    "OWNED",
    "SHARED",
]
```
## ListAvailableManagementCidrRangesPaginatorName

```python
# ListAvailableManagementCidrRangesPaginatorName usage example

from types_aiobotocore_workspaces.literals import ListAvailableManagementCidrRangesPaginatorName

def get_value() -> ListAvailableManagementCidrRangesPaginatorName:
    return "list_available_management_cidr_ranges"
```

```python
# ListAvailableManagementCidrRangesPaginatorName definition

ListAvailableManagementCidrRangesPaginatorName = Literal[
    "list_available_management_cidr_ranges",
]
```
## LogUploadEnumType

```python
# LogUploadEnumType usage example

from types_aiobotocore_workspaces.literals import LogUploadEnumType

def get_value() -> LogUploadEnumType:
    return "DISABLED"
```

```python
# LogUploadEnumType definition

LogUploadEnumType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ModificationResourceEnumType

```python
# ModificationResourceEnumType usage example

from types_aiobotocore_workspaces.literals import ModificationResourceEnumType

def get_value() -> ModificationResourceEnumType:
    return "COMPUTE_TYPE"
```

```python
# ModificationResourceEnumType definition

ModificationResourceEnumType = Literal[
    "COMPUTE_TYPE",
    "ROOT_VOLUME",
    "USER_VOLUME",
]
```
## ModificationStateEnumType

```python
# ModificationStateEnumType usage example

from types_aiobotocore_workspaces.literals import ModificationStateEnumType

def get_value() -> ModificationStateEnumType:
    return "UPDATE_INITIATED"
```

```python
# ModificationStateEnumType definition

ModificationStateEnumType = Literal[
    "UPDATE_IN_PROGRESS",
    "UPDATE_INITIATED",
]
```
## OperatingSystemTypeType

```python
# OperatingSystemTypeType usage example

from types_aiobotocore_workspaces.literals import OperatingSystemTypeType

def get_value() -> OperatingSystemTypeType:
    return "LINUX"
```

```python
# OperatingSystemTypeType definition

OperatingSystemTypeType = Literal[
    "LINUX",
    "WINDOWS",
]
```
## ProtocolType

```python
# ProtocolType usage example

from types_aiobotocore_workspaces.literals import ProtocolType

def get_value() -> ProtocolType:
    return "PCOIP"
```

```python
# ProtocolType definition

ProtocolType = Literal[
    "PCOIP",
    "WSP",
]
```
## ReconnectEnumType

```python
# ReconnectEnumType usage example

from types_aiobotocore_workspaces.literals import ReconnectEnumType

def get_value() -> ReconnectEnumType:
    return "DISABLED"
```

```python
# ReconnectEnumType definition

ReconnectEnumType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## RunningModeType

```python
# RunningModeType usage example

from types_aiobotocore_workspaces.literals import RunningModeType

def get_value() -> RunningModeType:
    return "ALWAYS_ON"
```

```python
# RunningModeType definition

RunningModeType = Literal[
    "ALWAYS_ON",
    "AUTO_STOP",
    "MANUAL",
]
```
## SamlStatusEnumType

```python
# SamlStatusEnumType usage example

from types_aiobotocore_workspaces.literals import SamlStatusEnumType

def get_value() -> SamlStatusEnumType:
    return "DISABLED"
```

```python
# SamlStatusEnumType definition

SamlStatusEnumType = Literal[
    "DISABLED",
    "ENABLED",
    "ENABLED_WITH_DIRECTORY_LOGIN_FALLBACK",
]
```
## StandbyWorkspaceRelationshipTypeType

```python
# StandbyWorkspaceRelationshipTypeType usage example

from types_aiobotocore_workspaces.literals import StandbyWorkspaceRelationshipTypeType

def get_value() -> StandbyWorkspaceRelationshipTypeType:
    return "PRIMARY"
```

```python
# StandbyWorkspaceRelationshipTypeType definition

StandbyWorkspaceRelationshipTypeType = Literal[
    "PRIMARY",
    "STANDBY",
]
```
## TargetWorkspaceStateType

```python
# TargetWorkspaceStateType usage example

from types_aiobotocore_workspaces.literals import TargetWorkspaceStateType

def get_value() -> TargetWorkspaceStateType:
    return "ADMIN_MAINTENANCE"
```

```python
# TargetWorkspaceStateType definition

TargetWorkspaceStateType = Literal[
    "ADMIN_MAINTENANCE",
    "AVAILABLE",
]
```
## TenancyType

```python
# TenancyType usage example

from types_aiobotocore_workspaces.literals import TenancyType

def get_value() -> TenancyType:
    return "DEDICATED"
```

```python
# TenancyType definition

TenancyType = Literal[
    "DEDICATED",
    "SHARED",
]
```
## WorkspaceBundleStateType

```python
# WorkspaceBundleStateType usage example

from types_aiobotocore_workspaces.literals import WorkspaceBundleStateType

def get_value() -> WorkspaceBundleStateType:
    return "AVAILABLE"
```

```python
# WorkspaceBundleStateType definition

WorkspaceBundleStateType = Literal[
    "AVAILABLE",
    "ERROR",
    "PENDING",
]
```
## WorkspaceDirectoryStateType

```python
# WorkspaceDirectoryStateType usage example

from types_aiobotocore_workspaces.literals import WorkspaceDirectoryStateType

def get_value() -> WorkspaceDirectoryStateType:
    return "DEREGISTERED"
```

```python
# WorkspaceDirectoryStateType definition

WorkspaceDirectoryStateType = Literal[
    "DEREGISTERED",
    "DEREGISTERING",
    "ERROR",
    "REGISTERED",
    "REGISTERING",
]
```
## WorkspaceDirectoryTypeType

```python
# WorkspaceDirectoryTypeType usage example

from types_aiobotocore_workspaces.literals import WorkspaceDirectoryTypeType

def get_value() -> WorkspaceDirectoryTypeType:
    return "AD_CONNECTOR"
```

```python
# WorkspaceDirectoryTypeType definition

WorkspaceDirectoryTypeType = Literal[
    "AD_CONNECTOR",
    "SIMPLE_AD",
]
```
## WorkspaceImageIngestionProcessType

```python
# WorkspaceImageIngestionProcessType usage example

from types_aiobotocore_workspaces.literals import WorkspaceImageIngestionProcessType

def get_value() -> WorkspaceImageIngestionProcessType:
    return "BYOL_GRAPHICS"
```

```python
# WorkspaceImageIngestionProcessType definition

WorkspaceImageIngestionProcessType = Literal[
    "BYOL_GRAPHICS",
    "BYOL_GRAPHICS_G4DN",
    "BYOL_GRAPHICS_G4DN_BYOP",
    "BYOL_GRAPHICSPRO",
    "BYOL_REGULAR",
    "BYOL_REGULAR_BYOP",
    "BYOL_REGULAR_WSP",
]
```
## WorkspaceImageRequiredTenancyType

```python
# WorkspaceImageRequiredTenancyType usage example

from types_aiobotocore_workspaces.literals import WorkspaceImageRequiredTenancyType

def get_value() -> WorkspaceImageRequiredTenancyType:
    return "DEDICATED"
```

```python
# WorkspaceImageRequiredTenancyType definition

WorkspaceImageRequiredTenancyType = Literal[
    "DEDICATED",
    "DEFAULT",
]
```
## WorkspaceImageStateType

```python
# WorkspaceImageStateType usage example

from types_aiobotocore_workspaces.literals import WorkspaceImageStateType

def get_value() -> WorkspaceImageStateType:
    return "AVAILABLE"
```

```python
# WorkspaceImageStateType definition

WorkspaceImageStateType = Literal[
    "AVAILABLE",
    "ERROR",
    "PENDING",
]
```
## WorkspaceStateType

```python
# WorkspaceStateType usage example

from types_aiobotocore_workspaces.literals import WorkspaceStateType

def get_value() -> WorkspaceStateType:
    return "ADMIN_MAINTENANCE"
```

```python
# WorkspaceStateType definition

WorkspaceStateType = Literal[
    "ADMIN_MAINTENANCE",
    "AVAILABLE",
    "ERROR",
    "IMPAIRED",
    "MAINTENANCE",
    "PENDING",
    "REBOOTING",
    "REBUILDING",
    "RESTORING",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "SUSPENDED",
    "TERMINATED",
    "TERMINATING",
    "UNHEALTHY",
    "UPDATING",
]
```
## WorkSpacesServiceName

```python
# WorkSpacesServiceName usage example

from types_aiobotocore_workspaces.literals import WorkSpacesServiceName

def get_value() -> WorkSpacesServiceName:
    return "workspaces"
```

```python
# WorkSpacesServiceName definition

WorkSpacesServiceName = Literal[
    "workspaces",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_workspaces.literals import ServiceName

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

from types_aiobotocore_workspaces.literals import ResourceServiceName

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

from types_aiobotocore_workspaces.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_account_modifications"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_account_modifications",
    "describe_ip_groups",
    "describe_workspace_bundles",
    "describe_workspace_directories",
    "describe_workspace_images",
    "describe_workspaces",
    "describe_workspaces_connection_status",
    "list_available_management_cidr_ranges",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_workspaces.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "sa-east-1",
    "us-east-1",
    "us-west-2",
]
```
