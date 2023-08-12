# Literals

> [Index](../README.md) > [EKS](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## AMITypesType

```python
# AMITypesType usage example

from types_aiobotocore_eks.literals import AMITypesType

def get_value() -> AMITypesType:
    return "AL2_ARM_64"
```

```python
# AMITypesType definition

AMITypesType = Literal[
    "AL2_ARM_64",
    "AL2_x86_64",
    "AL2_x86_64_GPU",
    "BOTTLEROCKET_ARM_64",
    "BOTTLEROCKET_ARM_64_NVIDIA",
    "BOTTLEROCKET_x86_64",
    "BOTTLEROCKET_x86_64_NVIDIA",
    "CUSTOM",
    "WINDOWS_CORE_2019_x86_64",
    "WINDOWS_CORE_2022_x86_64",
    "WINDOWS_FULL_2019_x86_64",
    "WINDOWS_FULL_2022_x86_64",
]
```
## AddonActiveWaiterName

```python
# AddonActiveWaiterName usage example

from types_aiobotocore_eks.literals import AddonActiveWaiterName

def get_value() -> AddonActiveWaiterName:
    return "addon_active"
```

```python
# AddonActiveWaiterName definition

AddonActiveWaiterName = Literal[
    "addon_active",
]
```
## AddonDeletedWaiterName

```python
# AddonDeletedWaiterName usage example

from types_aiobotocore_eks.literals import AddonDeletedWaiterName

def get_value() -> AddonDeletedWaiterName:
    return "addon_deleted"
```

```python
# AddonDeletedWaiterName definition

AddonDeletedWaiterName = Literal[
    "addon_deleted",
]
```
## AddonIssueCodeType

```python
# AddonIssueCodeType usage example

from types_aiobotocore_eks.literals import AddonIssueCodeType

def get_value() -> AddonIssueCodeType:
    return "AccessDenied"
```

```python
# AddonIssueCodeType definition

AddonIssueCodeType = Literal[
    "AccessDenied",
    "AdmissionRequestDenied",
    "ClusterUnreachable",
    "ConfigurationConflict",
    "InsufficientNumberOfReplicas",
    "InternalFailure",
    "K8sResourceNotFound",
    "UnsupportedAddonModification",
]
```
## AddonStatusType

```python
# AddonStatusType usage example

from types_aiobotocore_eks.literals import AddonStatusType

def get_value() -> AddonStatusType:
    return "ACTIVE"
```

```python
# AddonStatusType definition

AddonStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DEGRADED",
    "DELETE_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## CapacityTypesType

```python
# CapacityTypesType usage example

from types_aiobotocore_eks.literals import CapacityTypesType

def get_value() -> CapacityTypesType:
    return "ON_DEMAND"
```

```python
# CapacityTypesType definition

CapacityTypesType = Literal[
    "ON_DEMAND",
    "SPOT",
]
```
## ClusterActiveWaiterName

```python
# ClusterActiveWaiterName usage example

from types_aiobotocore_eks.literals import ClusterActiveWaiterName

def get_value() -> ClusterActiveWaiterName:
    return "cluster_active"
```

```python
# ClusterActiveWaiterName definition

ClusterActiveWaiterName = Literal[
    "cluster_active",
]
```
## ClusterDeletedWaiterName

```python
# ClusterDeletedWaiterName usage example

from types_aiobotocore_eks.literals import ClusterDeletedWaiterName

def get_value() -> ClusterDeletedWaiterName:
    return "cluster_deleted"
```

```python
# ClusterDeletedWaiterName definition

ClusterDeletedWaiterName = Literal[
    "cluster_deleted",
]
```
## ClusterIssueCodeType

```python
# ClusterIssueCodeType usage example

from types_aiobotocore_eks.literals import ClusterIssueCodeType

def get_value() -> ClusterIssueCodeType:
    return "AccessDenied"
```

```python
# ClusterIssueCodeType definition

ClusterIssueCodeType = Literal[
    "AccessDenied",
    "ClusterUnreachable",
    "ConfigurationConflict",
    "InternalFailure",
    "ResourceLimitExceeded",
    "ResourceNotFound",
]
```
## ClusterStatusType

```python
# ClusterStatusType usage example

from types_aiobotocore_eks.literals import ClusterStatusType

def get_value() -> ClusterStatusType:
    return "ACTIVE"
```

```python
# ClusterStatusType definition

ClusterStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "PENDING",
    "UPDATING",
]
```
## ConnectorConfigProviderType

```python
# ConnectorConfigProviderType usage example

from types_aiobotocore_eks.literals import ConnectorConfigProviderType

def get_value() -> ConnectorConfigProviderType:
    return "AKS"
```

```python
# ConnectorConfigProviderType definition

ConnectorConfigProviderType = Literal[
    "AKS",
    "ANTHOS",
    "EC2",
    "EKS_ANYWHERE",
    "GKE",
    "OPENSHIFT",
    "OTHER",
    "RANCHER",
    "TANZU",
]
```
## DescribeAddonVersionsPaginatorName

```python
# DescribeAddonVersionsPaginatorName usage example

from types_aiobotocore_eks.literals import DescribeAddonVersionsPaginatorName

def get_value() -> DescribeAddonVersionsPaginatorName:
    return "describe_addon_versions"
```

```python
# DescribeAddonVersionsPaginatorName definition

DescribeAddonVersionsPaginatorName = Literal[
    "describe_addon_versions",
]
```
## ErrorCodeType

```python
# ErrorCodeType usage example

from types_aiobotocore_eks.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "AccessDenied"
```

```python
# ErrorCodeType definition

ErrorCodeType = Literal[
    "AccessDenied",
    "AdmissionRequestDenied",
    "ClusterUnreachable",
    "ConfigurationConflict",
    "EniLimitReached",
    "InsufficientFreeAddresses",
    "InsufficientNumberOfReplicas",
    "IpNotAvailable",
    "K8sResourceNotFound",
    "NodeCreationFailure",
    "OperationNotPermitted",
    "PodEvictionFailure",
    "SecurityGroupNotFound",
    "SubnetNotFound",
    "Unknown",
    "UnsupportedAddonModification",
    "VpcIdNotFound",
]
```
## FargateProfileActiveWaiterName

```python
# FargateProfileActiveWaiterName usage example

from types_aiobotocore_eks.literals import FargateProfileActiveWaiterName

def get_value() -> FargateProfileActiveWaiterName:
    return "fargate_profile_active"
```

```python
# FargateProfileActiveWaiterName definition

FargateProfileActiveWaiterName = Literal[
    "fargate_profile_active",
]
```
## FargateProfileDeletedWaiterName

```python
# FargateProfileDeletedWaiterName usage example

from types_aiobotocore_eks.literals import FargateProfileDeletedWaiterName

def get_value() -> FargateProfileDeletedWaiterName:
    return "fargate_profile_deleted"
```

```python
# FargateProfileDeletedWaiterName definition

FargateProfileDeletedWaiterName = Literal[
    "fargate_profile_deleted",
]
```
## FargateProfileStatusType

```python
# FargateProfileStatusType usage example

from types_aiobotocore_eks.literals import FargateProfileStatusType

def get_value() -> FargateProfileStatusType:
    return "ACTIVE"
```

```python
# FargateProfileStatusType definition

FargateProfileStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
]
```
## IpFamilyType

```python
# IpFamilyType usage example

from types_aiobotocore_eks.literals import IpFamilyType

def get_value() -> IpFamilyType:
    return "ipv4"
```

```python
# IpFamilyType definition

IpFamilyType = Literal[
    "ipv4",
    "ipv6",
]
```
## ListAddonsPaginatorName

```python
# ListAddonsPaginatorName usage example

from types_aiobotocore_eks.literals import ListAddonsPaginatorName

def get_value() -> ListAddonsPaginatorName:
    return "list_addons"
```

```python
# ListAddonsPaginatorName definition

ListAddonsPaginatorName = Literal[
    "list_addons",
]
```
## ListClustersPaginatorName

```python
# ListClustersPaginatorName usage example

from types_aiobotocore_eks.literals import ListClustersPaginatorName

def get_value() -> ListClustersPaginatorName:
    return "list_clusters"
```

```python
# ListClustersPaginatorName definition

ListClustersPaginatorName = Literal[
    "list_clusters",
]
```
## ListFargateProfilesPaginatorName

```python
# ListFargateProfilesPaginatorName usage example

from types_aiobotocore_eks.literals import ListFargateProfilesPaginatorName

def get_value() -> ListFargateProfilesPaginatorName:
    return "list_fargate_profiles"
```

```python
# ListFargateProfilesPaginatorName definition

ListFargateProfilesPaginatorName = Literal[
    "list_fargate_profiles",
]
```
## ListIdentityProviderConfigsPaginatorName

```python
# ListIdentityProviderConfigsPaginatorName usage example

from types_aiobotocore_eks.literals import ListIdentityProviderConfigsPaginatorName

def get_value() -> ListIdentityProviderConfigsPaginatorName:
    return "list_identity_provider_configs"
```

```python
# ListIdentityProviderConfigsPaginatorName definition

ListIdentityProviderConfigsPaginatorName = Literal[
    "list_identity_provider_configs",
]
```
## ListNodegroupsPaginatorName

```python
# ListNodegroupsPaginatorName usage example

from types_aiobotocore_eks.literals import ListNodegroupsPaginatorName

def get_value() -> ListNodegroupsPaginatorName:
    return "list_nodegroups"
```

```python
# ListNodegroupsPaginatorName definition

ListNodegroupsPaginatorName = Literal[
    "list_nodegroups",
]
```
## ListUpdatesPaginatorName

```python
# ListUpdatesPaginatorName usage example

from types_aiobotocore_eks.literals import ListUpdatesPaginatorName

def get_value() -> ListUpdatesPaginatorName:
    return "list_updates"
```

```python
# ListUpdatesPaginatorName definition

ListUpdatesPaginatorName = Literal[
    "list_updates",
]
```
## LogTypeType

```python
# LogTypeType usage example

from types_aiobotocore_eks.literals import LogTypeType

def get_value() -> LogTypeType:
    return "api"
```

```python
# LogTypeType definition

LogTypeType = Literal[
    "api",
    "audit",
    "authenticator",
    "controllerManager",
    "scheduler",
]
```
## NodegroupActiveWaiterName

```python
# NodegroupActiveWaiterName usage example

from types_aiobotocore_eks.literals import NodegroupActiveWaiterName

def get_value() -> NodegroupActiveWaiterName:
    return "nodegroup_active"
```

```python
# NodegroupActiveWaiterName definition

NodegroupActiveWaiterName = Literal[
    "nodegroup_active",
]
```
## NodegroupDeletedWaiterName

```python
# NodegroupDeletedWaiterName usage example

from types_aiobotocore_eks.literals import NodegroupDeletedWaiterName

def get_value() -> NodegroupDeletedWaiterName:
    return "nodegroup_deleted"
```

```python
# NodegroupDeletedWaiterName definition

NodegroupDeletedWaiterName = Literal[
    "nodegroup_deleted",
]
```
## NodegroupIssueCodeType

```python
# NodegroupIssueCodeType usage example

from types_aiobotocore_eks.literals import NodegroupIssueCodeType

def get_value() -> NodegroupIssueCodeType:
    return "AccessDenied"
```

```python
# NodegroupIssueCodeType definition

NodegroupIssueCodeType = Literal[
    "AccessDenied",
    "AmiIdNotFound",
    "AsgInstanceLaunchFailures",
    "AutoScalingGroupInstanceRefreshActive",
    "AutoScalingGroupInvalidConfiguration",
    "AutoScalingGroupNotFound",
    "AutoScalingGroupOptInRequired",
    "AutoScalingGroupRateLimitExceeded",
    "ClusterUnreachable",
    "Ec2LaunchTemplateDeletionFailure",
    "Ec2LaunchTemplateInvalidConfiguration",
    "Ec2LaunchTemplateMaxLimitExceeded",
    "Ec2LaunchTemplateNotFound",
    "Ec2LaunchTemplateVersionMismatch",
    "Ec2SecurityGroupDeletionFailure",
    "Ec2SecurityGroupNotFound",
    "Ec2SubnetInvalidConfiguration",
    "Ec2SubnetListTooLong",
    "Ec2SubnetMissingIpv6Assignment",
    "Ec2SubnetNotFound",
    "IamInstanceProfileNotFound",
    "IamLimitExceeded",
    "IamNodeRoleNotFound",
    "IamThrottling",
    "InstanceLimitExceeded",
    "InsufficientFreeAddresses",
    "InternalFailure",
    "LimitExceeded",
    "NodeCreationFailure",
    "NodeTerminationFailure",
    "PodEvictionFailure",
    "SourceEc2LaunchTemplateNotFound",
    "Unknown",
]
```
## NodegroupStatusType

```python
# NodegroupStatusType usage example

from types_aiobotocore_eks.literals import NodegroupStatusType

def get_value() -> NodegroupStatusType:
    return "ACTIVE"
```

```python
# NodegroupStatusType definition

NodegroupStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DEGRADED",
    "DELETE_FAILED",
    "DELETING",
    "UPDATING",
]
```
## ResolveConflictsType

```python
# ResolveConflictsType usage example

from types_aiobotocore_eks.literals import ResolveConflictsType

def get_value() -> ResolveConflictsType:
    return "NONE"
```

```python
# ResolveConflictsType definition

ResolveConflictsType = Literal[
    "NONE",
    "OVERWRITE",
    "PRESERVE",
]
```
## TaintEffectType

```python
# TaintEffectType usage example

from types_aiobotocore_eks.literals import TaintEffectType

def get_value() -> TaintEffectType:
    return "NO_EXECUTE"
```

```python
# TaintEffectType definition

TaintEffectType = Literal[
    "NO_EXECUTE",
    "NO_SCHEDULE",
    "PREFER_NO_SCHEDULE",
]
```
## UpdateParamTypeType

```python
# UpdateParamTypeType usage example

from types_aiobotocore_eks.literals import UpdateParamTypeType

def get_value() -> UpdateParamTypeType:
    return "AddonVersion"
```

```python
# UpdateParamTypeType definition

UpdateParamTypeType = Literal[
    "AddonVersion",
    "ClusterLogging",
    "DesiredSize",
    "EncryptionConfig",
    "EndpointPrivateAccess",
    "EndpointPublicAccess",
    "IdentityProviderConfig",
    "LabelsToAdd",
    "LabelsToRemove",
    "LaunchTemplateName",
    "LaunchTemplateVersion",
    "MaxSize",
    "MaxUnavailable",
    "MaxUnavailablePercentage",
    "MinSize",
    "PlatformVersion",
    "PublicAccessCidrs",
    "ReleaseVersion",
    "ResolveConflicts",
    "ServiceAccountRoleArn",
    "TaintsToAdd",
    "TaintsToRemove",
    "Version",
]
```
## UpdateStatusType

```python
# UpdateStatusType usage example

from types_aiobotocore_eks.literals import UpdateStatusType

def get_value() -> UpdateStatusType:
    return "Cancelled"
```

```python
# UpdateStatusType definition

UpdateStatusType = Literal[
    "Cancelled",
    "Failed",
    "InProgress",
    "Successful",
]
```
## UpdateTypeType

```python
# UpdateTypeType usage example

from types_aiobotocore_eks.literals import UpdateTypeType

def get_value() -> UpdateTypeType:
    return "AddonUpdate"
```

```python
# UpdateTypeType definition

UpdateTypeType = Literal[
    "AddonUpdate",
    "AssociateEncryptionConfig",
    "AssociateIdentityProviderConfig",
    "ConfigUpdate",
    "DisassociateIdentityProviderConfig",
    "EndpointAccessUpdate",
    "LoggingUpdate",
    "VersionUpdate",
]
```
## configStatusType

```python
# configStatusType usage example

from types_aiobotocore_eks.literals import configStatusType

def get_value() -> configStatusType:
    return "ACTIVE"
```

```python
# configStatusType definition

configStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
]
```
## EKSServiceName

```python
# EKSServiceName usage example

from types_aiobotocore_eks.literals import EKSServiceName

def get_value() -> EKSServiceName:
    return "eks"
```

```python
# EKSServiceName definition

EKSServiceName = Literal[
    "eks",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_eks.literals import ServiceName

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

from types_aiobotocore_eks.literals import ResourceServiceName

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

from types_aiobotocore_eks.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_addon_versions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_addon_versions",
    "list_addons",
    "list_clusters",
    "list_fargate_profiles",
    "list_identity_provider_configs",
    "list_nodegroups",
    "list_updates",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_eks.literals import WaiterName

def get_value() -> WaiterName:
    return "addon_active"
```

```python
# WaiterName definition

WaiterName = Literal[
    "addon_active",
    "addon_deleted",
    "cluster_active",
    "cluster_deleted",
    "fargate_profile_active",
    "fargate_profile_deleted",
    "nodegroup_active",
    "nodegroup_deleted",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_eks.literals import RegionName

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
