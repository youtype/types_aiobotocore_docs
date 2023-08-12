# Literals

> [Index](../README.md) > [Backup](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## BackupJobStateType

```python
# BackupJobStateType usage example

from types_aiobotocore_backup.literals import BackupJobStateType

def get_value() -> BackupJobStateType:
    return "ABORTED"
```

```python
# BackupJobStateType definition

BackupJobStateType = Literal[
    "ABORTED",
    "ABORTING",
    "COMPLETED",
    "CREATED",
    "EXPIRED",
    "FAILED",
    "PARTIAL",
    "PENDING",
    "RUNNING",
]
```
## BackupVaultEventType

```python
# BackupVaultEventType usage example

from types_aiobotocore_backup.literals import BackupVaultEventType

def get_value() -> BackupVaultEventType:
    return "BACKUP_JOB_COMPLETED"
```

```python
# BackupVaultEventType definition

BackupVaultEventType = Literal[
    "BACKUP_JOB_COMPLETED",
    "BACKUP_JOB_EXPIRED",
    "BACKUP_JOB_FAILED",
    "BACKUP_JOB_STARTED",
    "BACKUP_JOB_SUCCESSFUL",
    "BACKUP_PLAN_CREATED",
    "BACKUP_PLAN_MODIFIED",
    "COPY_JOB_FAILED",
    "COPY_JOB_STARTED",
    "COPY_JOB_SUCCESSFUL",
    "RECOVERY_POINT_MODIFIED",
    "RESTORE_JOB_COMPLETED",
    "RESTORE_JOB_FAILED",
    "RESTORE_JOB_STARTED",
    "RESTORE_JOB_SUCCESSFUL",
    "S3_BACKUP_OBJECT_FAILED",
    "S3_RESTORE_OBJECT_FAILED",
]
```
## ConditionTypeType

```python
# ConditionTypeType usage example

from types_aiobotocore_backup.literals import ConditionTypeType

def get_value() -> ConditionTypeType:
    return "STRINGEQUALS"
```

```python
# ConditionTypeType definition

ConditionTypeType = Literal[
    "STRINGEQUALS",
]
```
## CopyJobStateType

```python
# CopyJobStateType usage example

from types_aiobotocore_backup.literals import CopyJobStateType

def get_value() -> CopyJobStateType:
    return "COMPLETED"
```

```python
# CopyJobStateType definition

CopyJobStateType = Literal[
    "COMPLETED",
    "CREATED",
    "FAILED",
    "PARTIAL",
    "RUNNING",
]
```
## LegalHoldStatusType

```python
# LegalHoldStatusType usage example

from types_aiobotocore_backup.literals import LegalHoldStatusType

def get_value() -> LegalHoldStatusType:
    return "ACTIVE"
```

```python
# LegalHoldStatusType definition

LegalHoldStatusType = Literal[
    "ACTIVE",
    "CANCELED",
    "CANCELING",
    "CREATING",
]
```
## ListBackupJobsPaginatorName

```python
# ListBackupJobsPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupJobsPaginatorName

def get_value() -> ListBackupJobsPaginatorName:
    return "list_backup_jobs"
```

```python
# ListBackupJobsPaginatorName definition

ListBackupJobsPaginatorName = Literal[
    "list_backup_jobs",
]
```
## ListBackupPlanTemplatesPaginatorName

```python
# ListBackupPlanTemplatesPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupPlanTemplatesPaginatorName

def get_value() -> ListBackupPlanTemplatesPaginatorName:
    return "list_backup_plan_templates"
```

```python
# ListBackupPlanTemplatesPaginatorName definition

ListBackupPlanTemplatesPaginatorName = Literal[
    "list_backup_plan_templates",
]
```
## ListBackupPlanVersionsPaginatorName

```python
# ListBackupPlanVersionsPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupPlanVersionsPaginatorName

def get_value() -> ListBackupPlanVersionsPaginatorName:
    return "list_backup_plan_versions"
```

```python
# ListBackupPlanVersionsPaginatorName definition

ListBackupPlanVersionsPaginatorName = Literal[
    "list_backup_plan_versions",
]
```
## ListBackupPlansPaginatorName

```python
# ListBackupPlansPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupPlansPaginatorName

def get_value() -> ListBackupPlansPaginatorName:
    return "list_backup_plans"
```

```python
# ListBackupPlansPaginatorName definition

ListBackupPlansPaginatorName = Literal[
    "list_backup_plans",
]
```
## ListBackupSelectionsPaginatorName

```python
# ListBackupSelectionsPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupSelectionsPaginatorName

def get_value() -> ListBackupSelectionsPaginatorName:
    return "list_backup_selections"
```

```python
# ListBackupSelectionsPaginatorName definition

ListBackupSelectionsPaginatorName = Literal[
    "list_backup_selections",
]
```
## ListBackupVaultsPaginatorName

```python
# ListBackupVaultsPaginatorName usage example

from types_aiobotocore_backup.literals import ListBackupVaultsPaginatorName

def get_value() -> ListBackupVaultsPaginatorName:
    return "list_backup_vaults"
```

```python
# ListBackupVaultsPaginatorName definition

ListBackupVaultsPaginatorName = Literal[
    "list_backup_vaults",
]
```
## ListCopyJobsPaginatorName

```python
# ListCopyJobsPaginatorName usage example

from types_aiobotocore_backup.literals import ListCopyJobsPaginatorName

def get_value() -> ListCopyJobsPaginatorName:
    return "list_copy_jobs"
```

```python
# ListCopyJobsPaginatorName definition

ListCopyJobsPaginatorName = Literal[
    "list_copy_jobs",
]
```
## ListLegalHoldsPaginatorName

```python
# ListLegalHoldsPaginatorName usage example

from types_aiobotocore_backup.literals import ListLegalHoldsPaginatorName

def get_value() -> ListLegalHoldsPaginatorName:
    return "list_legal_holds"
```

```python
# ListLegalHoldsPaginatorName definition

ListLegalHoldsPaginatorName = Literal[
    "list_legal_holds",
]
```
## ListProtectedResourcesByBackupVaultPaginatorName

```python
# ListProtectedResourcesByBackupVaultPaginatorName usage example

from types_aiobotocore_backup.literals import ListProtectedResourcesByBackupVaultPaginatorName

def get_value() -> ListProtectedResourcesByBackupVaultPaginatorName:
    return "list_protected_resources_by_backup_vault"
```

```python
# ListProtectedResourcesByBackupVaultPaginatorName definition

ListProtectedResourcesByBackupVaultPaginatorName = Literal[
    "list_protected_resources_by_backup_vault",
]
```
## ListProtectedResourcesPaginatorName

```python
# ListProtectedResourcesPaginatorName usage example

from types_aiobotocore_backup.literals import ListProtectedResourcesPaginatorName

def get_value() -> ListProtectedResourcesPaginatorName:
    return "list_protected_resources"
```

```python
# ListProtectedResourcesPaginatorName definition

ListProtectedResourcesPaginatorName = Literal[
    "list_protected_resources",
]
```
## ListRecoveryPointsByBackupVaultPaginatorName

```python
# ListRecoveryPointsByBackupVaultPaginatorName usage example

from types_aiobotocore_backup.literals import ListRecoveryPointsByBackupVaultPaginatorName

def get_value() -> ListRecoveryPointsByBackupVaultPaginatorName:
    return "list_recovery_points_by_backup_vault"
```

```python
# ListRecoveryPointsByBackupVaultPaginatorName definition

ListRecoveryPointsByBackupVaultPaginatorName = Literal[
    "list_recovery_points_by_backup_vault",
]
```
## ListRecoveryPointsByLegalHoldPaginatorName

```python
# ListRecoveryPointsByLegalHoldPaginatorName usage example

from types_aiobotocore_backup.literals import ListRecoveryPointsByLegalHoldPaginatorName

def get_value() -> ListRecoveryPointsByLegalHoldPaginatorName:
    return "list_recovery_points_by_legal_hold"
```

```python
# ListRecoveryPointsByLegalHoldPaginatorName definition

ListRecoveryPointsByLegalHoldPaginatorName = Literal[
    "list_recovery_points_by_legal_hold",
]
```
## ListRecoveryPointsByResourcePaginatorName

```python
# ListRecoveryPointsByResourcePaginatorName usage example

from types_aiobotocore_backup.literals import ListRecoveryPointsByResourcePaginatorName

def get_value() -> ListRecoveryPointsByResourcePaginatorName:
    return "list_recovery_points_by_resource"
```

```python
# ListRecoveryPointsByResourcePaginatorName definition

ListRecoveryPointsByResourcePaginatorName = Literal[
    "list_recovery_points_by_resource",
]
```
## ListRestoreJobsPaginatorName

```python
# ListRestoreJobsPaginatorName usage example

from types_aiobotocore_backup.literals import ListRestoreJobsPaginatorName

def get_value() -> ListRestoreJobsPaginatorName:
    return "list_restore_jobs"
```

```python
# ListRestoreJobsPaginatorName definition

ListRestoreJobsPaginatorName = Literal[
    "list_restore_jobs",
]
```
## RecoveryPointStatusType

```python
# RecoveryPointStatusType usage example

from types_aiobotocore_backup.literals import RecoveryPointStatusType

def get_value() -> RecoveryPointStatusType:
    return "COMPLETED"
```

```python
# RecoveryPointStatusType definition

RecoveryPointStatusType = Literal[
    "COMPLETED",
    "DELETING",
    "EXPIRED",
    "PARTIAL",
]
```
## RestoreJobStatusType

```python
# RestoreJobStatusType usage example

from types_aiobotocore_backup.literals import RestoreJobStatusType

def get_value() -> RestoreJobStatusType:
    return "ABORTED"
```

```python
# RestoreJobStatusType definition

RestoreJobStatusType = Literal[
    "ABORTED",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "RUNNING",
]
```
## StorageClassType

```python
# StorageClassType usage example

from types_aiobotocore_backup.literals import StorageClassType

def get_value() -> StorageClassType:
    return "COLD"
```

```python
# StorageClassType definition

StorageClassType = Literal[
    "COLD",
    "DELETED",
    "WARM",
]
```
## VaultStateType

```python
# VaultStateType usage example

from types_aiobotocore_backup.literals import VaultStateType

def get_value() -> VaultStateType:
    return "AVAILABLE"
```

```python
# VaultStateType definition

VaultStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "FAILED",
]
```
## VaultTypeType

```python
# VaultTypeType usage example

from types_aiobotocore_backup.literals import VaultTypeType

def get_value() -> VaultTypeType:
    return "BACKUP_VAULT"
```

```python
# VaultTypeType definition

VaultTypeType = Literal[
    "BACKUP_VAULT",
    "LOGICALLY_AIR_GAPPED_BACKUP_VAULT",
]
```
## BackupServiceName

```python
# BackupServiceName usage example

from types_aiobotocore_backup.literals import BackupServiceName

def get_value() -> BackupServiceName:
    return "backup"
```

```python
# BackupServiceName definition

BackupServiceName = Literal[
    "backup",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_backup.literals import ServiceName

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

from types_aiobotocore_backup.literals import ResourceServiceName

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

from types_aiobotocore_backup.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_backup_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_backup_jobs",
    "list_backup_plan_templates",
    "list_backup_plan_versions",
    "list_backup_plans",
    "list_backup_selections",
    "list_backup_vaults",
    "list_copy_jobs",
    "list_legal_holds",
    "list_protected_resources",
    "list_protected_resources_by_backup_vault",
    "list_recovery_points_by_backup_vault",
    "list_recovery_points_by_legal_hold",
    "list_recovery_points_by_resource",
    "list_restore_jobs",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_backup.literals import RegionName

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
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
