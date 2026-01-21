# Literals

> [Index](../README.md) > [Mgn](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## ActionCategoryType

```python
# ActionCategoryType usage example
from types_aiobotocore_mgn.literals import ActionCategoryType

def get_value() -> ActionCategoryType:
    return "BACKUP"
```

```python
# ActionCategoryType definition
ActionCategoryType = Literal[
    "BACKUP",
    "CONFIGURATION",
    "DISASTER_RECOVERY",
    "LICENSE_AND_SUBSCRIPTION",
    "NETWORKING",
    "OBSERVABILITY",
    "OPERATING_SYSTEM",
    "OTHER",
    "REFACTORING",
    "SECURITY",
    "VALIDATION",
]
```
## ApplicationHealthStatusType

```python
# ApplicationHealthStatusType usage example
from types_aiobotocore_mgn.literals import ApplicationHealthStatusType

def get_value() -> ApplicationHealthStatusType:
    return "ERROR"
```

```python
# ApplicationHealthStatusType definition
ApplicationHealthStatusType = Literal[
    "ERROR",
    "HEALTHY",
    "LAGGING",
]
```
## ApplicationProgressStatusType

```python
# ApplicationProgressStatusType usage example
from types_aiobotocore_mgn.literals import ApplicationProgressStatusType

def get_value() -> ApplicationProgressStatusType:
    return "COMPLETED"
```

```python
# ApplicationProgressStatusType definition
ApplicationProgressStatusType = Literal[
    "COMPLETED",
    "IN_PROGRESS",
    "NOT_STARTED",
]
```
## BootModeType

```python
# BootModeType usage example
from types_aiobotocore_mgn.literals import BootModeType

def get_value() -> BootModeType:
    return "LEGACY_BIOS"
```

```python
# BootModeType definition
BootModeType = Literal[
    "LEGACY_BIOS",
    "UEFI",
    "USE_SOURCE",
]
```
## ChangeServerLifeCycleStateSourceServerLifecycleStateType

```python
# ChangeServerLifeCycleStateSourceServerLifecycleStateType usage example
from types_aiobotocore_mgn.literals import ChangeServerLifeCycleStateSourceServerLifecycleStateType

def get_value() -> ChangeServerLifeCycleStateSourceServerLifecycleStateType:
    return "CUTOVER"
```

```python
# ChangeServerLifeCycleStateSourceServerLifecycleStateType definition
ChangeServerLifeCycleStateSourceServerLifecycleStateType = Literal[
    "CUTOVER",
    "READY_FOR_CUTOVER",
    "READY_FOR_TEST",
]
```
## DataReplicationErrorStringType

```python
# DataReplicationErrorStringType usage example
from types_aiobotocore_mgn.literals import DataReplicationErrorStringType

def get_value() -> DataReplicationErrorStringType:
    return "AGENT_NOT_SEEN"
```

```python
# DataReplicationErrorStringType definition
DataReplicationErrorStringType = Literal[
    "AGENT_NOT_SEEN",
    "FAILED_TO_ATTACH_STAGING_DISKS",
    "FAILED_TO_AUTHENTICATE_WITH_SERVICE",
    "FAILED_TO_BOOT_REPLICATION_SERVER",
    "FAILED_TO_CONNECT_AGENT_TO_REPLICATION_SERVER",
    "FAILED_TO_CREATE_SECURITY_GROUP",
    "FAILED_TO_CREATE_STAGING_DISKS",
    "FAILED_TO_DOWNLOAD_REPLICATION_SOFTWARE",
    "FAILED_TO_LAUNCH_REPLICATION_SERVER",
    "FAILED_TO_PAIR_REPLICATION_SERVER_WITH_AGENT",
    "FAILED_TO_START_DATA_TRANSFER",
    "LAST_SNAPSHOT_JOB_FAILED",
    "NOT_CONVERGING",
    "SNAPSHOTS_FAILURE",
    "UNSTABLE_NETWORK",
    "UNSUPPORTED_VM_CONFIGURATION",
]
```
## DataReplicationInitiationStepNameType

```python
# DataReplicationInitiationStepNameType usage example
from types_aiobotocore_mgn.literals import DataReplicationInitiationStepNameType

def get_value() -> DataReplicationInitiationStepNameType:
    return "ATTACH_STAGING_DISKS"
```

```python
# DataReplicationInitiationStepNameType definition
DataReplicationInitiationStepNameType = Literal[
    "ATTACH_STAGING_DISKS",
    "AUTHENTICATE_WITH_SERVICE",
    "BOOT_REPLICATION_SERVER",
    "CONNECT_AGENT_TO_REPLICATION_SERVER",
    "CREATE_SECURITY_GROUP",
    "CREATE_STAGING_DISKS",
    "DOWNLOAD_REPLICATION_SOFTWARE",
    "LAUNCH_REPLICATION_SERVER",
    "PAIR_REPLICATION_SERVER_WITH_AGENT",
    "START_DATA_TRANSFER",
    "WAIT",
]
```
## DataReplicationInitiationStepStatusType

```python
# DataReplicationInitiationStepStatusType usage example
from types_aiobotocore_mgn.literals import DataReplicationInitiationStepStatusType

def get_value() -> DataReplicationInitiationStepStatusType:
    return "FAILED"
```

```python
# DataReplicationInitiationStepStatusType definition
DataReplicationInitiationStepStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "NOT_STARTED",
    "SKIPPED",
    "SUCCEEDED",
]
```
## DataReplicationStateType

```python
# DataReplicationStateType usage example
from types_aiobotocore_mgn.literals import DataReplicationStateType

def get_value() -> DataReplicationStateType:
    return "BACKLOG"
```

```python
# DataReplicationStateType definition
DataReplicationStateType = Literal[
    "BACKLOG",
    "CONTINUOUS",
    "CREATING_SNAPSHOT",
    "DISCONNECTED",
    "INITIAL_SYNC",
    "INITIATING",
    "PAUSED",
    "PENDING_SNAPSHOT_SHIPPING",
    "RESCAN",
    "SHIPPING_SNAPSHOT",
    "STALLED",
    "STOPPED",
]
```
## DescribeJobLogItemsPaginatorName

```python
# DescribeJobLogItemsPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeJobLogItemsPaginatorName

def get_value() -> DescribeJobLogItemsPaginatorName:
    return "describe_job_log_items"
```

```python
# DescribeJobLogItemsPaginatorName definition
DescribeJobLogItemsPaginatorName = Literal[
    "describe_job_log_items",
]
```
## DescribeJobsPaginatorName

```python
# DescribeJobsPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeJobsPaginatorName

def get_value() -> DescribeJobsPaginatorName:
    return "describe_jobs"
```

```python
# DescribeJobsPaginatorName definition
DescribeJobsPaginatorName = Literal[
    "describe_jobs",
]
```
## DescribeLaunchConfigurationTemplatesPaginatorName

```python
# DescribeLaunchConfigurationTemplatesPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeLaunchConfigurationTemplatesPaginatorName

def get_value() -> DescribeLaunchConfigurationTemplatesPaginatorName:
    return "describe_launch_configuration_templates"
```

```python
# DescribeLaunchConfigurationTemplatesPaginatorName definition
DescribeLaunchConfigurationTemplatesPaginatorName = Literal[
    "describe_launch_configuration_templates",
]
```
## DescribeReplicationConfigurationTemplatesPaginatorName

```python
# DescribeReplicationConfigurationTemplatesPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeReplicationConfigurationTemplatesPaginatorName

def get_value() -> DescribeReplicationConfigurationTemplatesPaginatorName:
    return "describe_replication_configuration_templates"
```

```python
# DescribeReplicationConfigurationTemplatesPaginatorName definition
DescribeReplicationConfigurationTemplatesPaginatorName = Literal[
    "describe_replication_configuration_templates",
]
```
## DescribeSourceServersPaginatorName

```python
# DescribeSourceServersPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeSourceServersPaginatorName

def get_value() -> DescribeSourceServersPaginatorName:
    return "describe_source_servers"
```

```python
# DescribeSourceServersPaginatorName definition
DescribeSourceServersPaginatorName = Literal[
    "describe_source_servers",
]
```
## DescribeVcenterClientsPaginatorName

```python
# DescribeVcenterClientsPaginatorName usage example
from types_aiobotocore_mgn.literals import DescribeVcenterClientsPaginatorName

def get_value() -> DescribeVcenterClientsPaginatorName:
    return "describe_vcenter_clients"
```

```python
# DescribeVcenterClientsPaginatorName definition
DescribeVcenterClientsPaginatorName = Literal[
    "describe_vcenter_clients",
]
```
## ExportStatusType

```python
# ExportStatusType usage example
from types_aiobotocore_mgn.literals import ExportStatusType

def get_value() -> ExportStatusType:
    return "FAILED"
```

```python
# ExportStatusType definition
ExportStatusType = Literal[
    "FAILED",
    "PENDING",
    "STARTED",
    "SUCCEEDED",
]
```
## FirstBootType

```python
# FirstBootType usage example
from types_aiobotocore_mgn.literals import FirstBootType

def get_value() -> FirstBootType:
    return "STOPPED"
```

```python
# FirstBootType definition
FirstBootType = Literal[
    "STOPPED",
    "SUCCEEDED",
    "UNKNOWN",
    "WAITING",
]
```
## ImportErrorTypeType

```python
# ImportErrorTypeType usage example
from types_aiobotocore_mgn.literals import ImportErrorTypeType

def get_value() -> ImportErrorTypeType:
    return "PROCESSING_ERROR"
```

```python
# ImportErrorTypeType definition
ImportErrorTypeType = Literal[
    "PROCESSING_ERROR",
    "VALIDATION_ERROR",
]
```
## ImportStatusType

```python
# ImportStatusType usage example
from types_aiobotocore_mgn.literals import ImportStatusType

def get_value() -> ImportStatusType:
    return "FAILED"
```

```python
# ImportStatusType definition
ImportStatusType = Literal[
    "FAILED",
    "PENDING",
    "STARTED",
    "SUCCEEDED",
]
```
## InitiatedByType

```python
# InitiatedByType usage example
from types_aiobotocore_mgn.literals import InitiatedByType

def get_value() -> InitiatedByType:
    return "DIAGNOSTIC"
```

```python
# InitiatedByType definition
InitiatedByType = Literal[
    "DIAGNOSTIC",
    "START_CUTOVER",
    "START_TEST",
    "TERMINATE",
]
```
## InternetProtocolType

```python
# InternetProtocolType usage example
from types_aiobotocore_mgn.literals import InternetProtocolType

def get_value() -> InternetProtocolType:
    return "IPV4"
```

```python
# InternetProtocolType definition
InternetProtocolType = Literal[
    "IPV4",
    "IPV6",
]
```
## JobLogEventType

```python
# JobLogEventType usage example
from types_aiobotocore_mgn.literals import JobLogEventType

def get_value() -> JobLogEventType:
    return "CLEANUP_END"
```

```python
# JobLogEventType definition
JobLogEventType = Literal[
    "CLEANUP_END",
    "CLEANUP_FAIL",
    "CLEANUP_START",
    "CONVERSION_END",
    "CONVERSION_FAIL",
    "CONVERSION_START",
    "JOB_CANCEL",
    "JOB_END",
    "JOB_START",
    "LAUNCH_FAILED",
    "LAUNCH_START",
    "SERVER_SKIPPED",
    "SNAPSHOT_END",
    "SNAPSHOT_FAIL",
    "SNAPSHOT_START",
    "USING_PREVIOUS_SNAPSHOT",
]
```
## JobStatusType

```python
# JobStatusType usage example
from types_aiobotocore_mgn.literals import JobStatusType

def get_value() -> JobStatusType:
    return "COMPLETED"
```

```python
# JobStatusType definition
JobStatusType = Literal[
    "COMPLETED",
    "PENDING",
    "STARTED",
]
```
## JobTypeType

```python
# JobTypeType usage example
from types_aiobotocore_mgn.literals import JobTypeType

def get_value() -> JobTypeType:
    return "LAUNCH"
```

```python
# JobTypeType definition
JobTypeType = Literal[
    "LAUNCH",
    "TERMINATE",
]
```
## LaunchDispositionType

```python
# LaunchDispositionType usage example
from types_aiobotocore_mgn.literals import LaunchDispositionType

def get_value() -> LaunchDispositionType:
    return "STARTED"
```

```python
# LaunchDispositionType definition
LaunchDispositionType = Literal[
    "STARTED",
    "STOPPED",
]
```
## LaunchStatusType

```python
# LaunchStatusType usage example
from types_aiobotocore_mgn.literals import LaunchStatusType

def get_value() -> LaunchStatusType:
    return "FAILED"
```

```python
# LaunchStatusType definition
LaunchStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "LAUNCHED",
    "PENDING",
    "TERMINATED",
]
```
## LifeCycleStateType

```python
# LifeCycleStateType usage example
from types_aiobotocore_mgn.literals import LifeCycleStateType

def get_value() -> LifeCycleStateType:
    return "CUTOVER"
```

```python
# LifeCycleStateType definition
LifeCycleStateType = Literal[
    "CUTOVER",
    "CUTTING_OVER",
    "DISCONNECTED",
    "DISCOVERED",
    "NOT_READY",
    "PENDING_INSTALLATION",
    "READY_FOR_CUTOVER",
    "READY_FOR_TEST",
    "STOPPED",
    "TESTING",
]
```
## ListApplicationsPaginatorName

```python
# ListApplicationsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python
# ListApplicationsPaginatorName definition
ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListConnectorsPaginatorName

```python
# ListConnectorsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListConnectorsPaginatorName

def get_value() -> ListConnectorsPaginatorName:
    return "list_connectors"
```

```python
# ListConnectorsPaginatorName definition
ListConnectorsPaginatorName = Literal[
    "list_connectors",
]
```
## ListExportErrorsPaginatorName

```python
# ListExportErrorsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListExportErrorsPaginatorName

def get_value() -> ListExportErrorsPaginatorName:
    return "list_export_errors"
```

```python
# ListExportErrorsPaginatorName definition
ListExportErrorsPaginatorName = Literal[
    "list_export_errors",
]
```
## ListExportsPaginatorName

```python
# ListExportsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListExportsPaginatorName

def get_value() -> ListExportsPaginatorName:
    return "list_exports"
```

```python
# ListExportsPaginatorName definition
ListExportsPaginatorName = Literal[
    "list_exports",
]
```
## ListImportErrorsPaginatorName

```python
# ListImportErrorsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListImportErrorsPaginatorName

def get_value() -> ListImportErrorsPaginatorName:
    return "list_import_errors"
```

```python
# ListImportErrorsPaginatorName definition
ListImportErrorsPaginatorName = Literal[
    "list_import_errors",
]
```
## ListImportsPaginatorName

```python
# ListImportsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListImportsPaginatorName

def get_value() -> ListImportsPaginatorName:
    return "list_imports"
```

```python
# ListImportsPaginatorName definition
ListImportsPaginatorName = Literal[
    "list_imports",
]
```
## ListManagedAccountsPaginatorName

```python
# ListManagedAccountsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListManagedAccountsPaginatorName

def get_value() -> ListManagedAccountsPaginatorName:
    return "list_managed_accounts"
```

```python
# ListManagedAccountsPaginatorName definition
ListManagedAccountsPaginatorName = Literal[
    "list_managed_accounts",
]
```
## ListSourceServerActionsPaginatorName

```python
# ListSourceServerActionsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListSourceServerActionsPaginatorName

def get_value() -> ListSourceServerActionsPaginatorName:
    return "list_source_server_actions"
```

```python
# ListSourceServerActionsPaginatorName definition
ListSourceServerActionsPaginatorName = Literal[
    "list_source_server_actions",
]
```
## ListTemplateActionsPaginatorName

```python
# ListTemplateActionsPaginatorName usage example
from types_aiobotocore_mgn.literals import ListTemplateActionsPaginatorName

def get_value() -> ListTemplateActionsPaginatorName:
    return "list_template_actions"
```

```python
# ListTemplateActionsPaginatorName definition
ListTemplateActionsPaginatorName = Literal[
    "list_template_actions",
]
```
## ListWavesPaginatorName

```python
# ListWavesPaginatorName usage example
from types_aiobotocore_mgn.literals import ListWavesPaginatorName

def get_value() -> ListWavesPaginatorName:
    return "list_waves"
```

```python
# ListWavesPaginatorName definition
ListWavesPaginatorName = Literal[
    "list_waves",
]
```
## PostLaunchActionExecutionStatusType

```python
# PostLaunchActionExecutionStatusType usage example
from types_aiobotocore_mgn.literals import PostLaunchActionExecutionStatusType

def get_value() -> PostLaunchActionExecutionStatusType:
    return "FAILED"
```

```python
# PostLaunchActionExecutionStatusType definition
PostLaunchActionExecutionStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## PostLaunchActionsDeploymentTypeType

```python
# PostLaunchActionsDeploymentTypeType usage example
from types_aiobotocore_mgn.literals import PostLaunchActionsDeploymentTypeType

def get_value() -> PostLaunchActionsDeploymentTypeType:
    return "CUTOVER_ONLY"
```

```python
# PostLaunchActionsDeploymentTypeType definition
PostLaunchActionsDeploymentTypeType = Literal[
    "CUTOVER_ONLY",
    "TEST_AND_CUTOVER",
    "TEST_ONLY",
]
```
## ReplicationConfigurationDataPlaneRoutingType

```python
# ReplicationConfigurationDataPlaneRoutingType usage example
from types_aiobotocore_mgn.literals import ReplicationConfigurationDataPlaneRoutingType

def get_value() -> ReplicationConfigurationDataPlaneRoutingType:
    return "PRIVATE_IP"
```

```python
# ReplicationConfigurationDataPlaneRoutingType definition
ReplicationConfigurationDataPlaneRoutingType = Literal[
    "PRIVATE_IP",
    "PUBLIC_IP",
]
```
## ReplicationConfigurationDefaultLargeStagingDiskTypeType

```python
# ReplicationConfigurationDefaultLargeStagingDiskTypeType usage example
from types_aiobotocore_mgn.literals import ReplicationConfigurationDefaultLargeStagingDiskTypeType

def get_value() -> ReplicationConfigurationDefaultLargeStagingDiskTypeType:
    return "GP2"
```

```python
# ReplicationConfigurationDefaultLargeStagingDiskTypeType definition
ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal[
    "GP2",
    "GP3",
    "ST1",
]
```
## ReplicationConfigurationEbsEncryptionType

```python
# ReplicationConfigurationEbsEncryptionType usage example
from types_aiobotocore_mgn.literals import ReplicationConfigurationEbsEncryptionType

def get_value() -> ReplicationConfigurationEbsEncryptionType:
    return "CUSTOM"
```

```python
# ReplicationConfigurationEbsEncryptionType definition
ReplicationConfigurationEbsEncryptionType = Literal[
    "CUSTOM",
    "DEFAULT",
]
```
## ReplicationConfigurationReplicatedDiskStagingDiskTypeType

```python
# ReplicationConfigurationReplicatedDiskStagingDiskTypeType usage example
from types_aiobotocore_mgn.literals import ReplicationConfigurationReplicatedDiskStagingDiskTypeType

def get_value() -> ReplicationConfigurationReplicatedDiskStagingDiskTypeType:
    return "AUTO"
```

```python
# ReplicationConfigurationReplicatedDiskStagingDiskTypeType definition
ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
    "AUTO",
    "GP2",
    "GP3",
    "IO1",
    "IO2",
    "SC1",
    "ST1",
    "STANDARD",
]
```
## ReplicationTypeType

```python
# ReplicationTypeType usage example
from types_aiobotocore_mgn.literals import ReplicationTypeType

def get_value() -> ReplicationTypeType:
    return "AGENT_BASED"
```

```python
# ReplicationTypeType definition
ReplicationTypeType = Literal[
    "AGENT_BASED",
    "SNAPSHOT_SHIPPING",
]
```
## SsmDocumentTypeType

```python
# SsmDocumentTypeType usage example
from types_aiobotocore_mgn.literals import SsmDocumentTypeType

def get_value() -> SsmDocumentTypeType:
    return "AUTOMATION"
```

```python
# SsmDocumentTypeType definition
SsmDocumentTypeType = Literal[
    "AUTOMATION",
    "COMMAND",
]
```
## SsmParameterStoreParameterTypeType

```python
# SsmParameterStoreParameterTypeType usage example
from types_aiobotocore_mgn.literals import SsmParameterStoreParameterTypeType

def get_value() -> SsmParameterStoreParameterTypeType:
    return "SECURE_STRING"
```

```python
# SsmParameterStoreParameterTypeType definition
SsmParameterStoreParameterTypeType = Literal[
    "SECURE_STRING",
    "STRING",
]
```
## TargetInstanceTypeRightSizingMethodType

```python
# TargetInstanceTypeRightSizingMethodType usage example
from types_aiobotocore_mgn.literals import TargetInstanceTypeRightSizingMethodType

def get_value() -> TargetInstanceTypeRightSizingMethodType:
    return "BASIC"
```

```python
# TargetInstanceTypeRightSizingMethodType definition
TargetInstanceTypeRightSizingMethodType = Literal[
    "BASIC",
    "NONE",
]
```
## VolumeTypeType

```python
# VolumeTypeType usage example
from types_aiobotocore_mgn.literals import VolumeTypeType

def get_value() -> VolumeTypeType:
    return "gp2"
```

```python
# VolumeTypeType definition
VolumeTypeType = Literal[
    "gp2",
    "gp3",
    "io1",
    "io2",
    "sc1",
    "st1",
    "standard",
]
```
## WaveHealthStatusType

```python
# WaveHealthStatusType usage example
from types_aiobotocore_mgn.literals import WaveHealthStatusType

def get_value() -> WaveHealthStatusType:
    return "ERROR"
```

```python
# WaveHealthStatusType definition
WaveHealthStatusType = Literal[
    "ERROR",
    "HEALTHY",
    "LAGGING",
]
```
## WaveProgressStatusType

```python
# WaveProgressStatusType usage example
from types_aiobotocore_mgn.literals import WaveProgressStatusType

def get_value() -> WaveProgressStatusType:
    return "COMPLETED"
```

```python
# WaveProgressStatusType definition
WaveProgressStatusType = Literal[
    "COMPLETED",
    "IN_PROGRESS",
    "NOT_STARTED",
]
```
## MgnServiceName

```python
# MgnServiceName usage example
from types_aiobotocore_mgn.literals import MgnServiceName

def get_value() -> MgnServiceName:
    return "mgn"
```

```python
# MgnServiceName definition
MgnServiceName = Literal[
    "mgn",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_mgn.literals import ServiceName

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
from types_aiobotocore_mgn.literals import ResourceServiceName

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
from types_aiobotocore_mgn.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_job_log_items"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_job_log_items",
    "describe_jobs",
    "describe_launch_configuration_templates",
    "describe_replication_configuration_templates",
    "describe_source_servers",
    "describe_vcenter_clients",
    "list_applications",
    "list_connectors",
    "list_export_errors",
    "list_exports",
    "list_import_errors",
    "list_imports",
    "list_managed_accounts",
    "list_source_server_actions",
    "list_template_actions",
    "list_waves",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_mgn.literals import RegionName

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
    "ap-southeast-5",
    "ap-southeast-7",
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
