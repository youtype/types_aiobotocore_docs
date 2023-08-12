# Literals

> [Index](../README.md) > [SsmSap](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).

## ApplicationDiscoveryStatusType

```python
# ApplicationDiscoveryStatusType usage example

from types_aiobotocore_ssm_sap.literals import ApplicationDiscoveryStatusType

def get_value() -> ApplicationDiscoveryStatusType:
    return "DELETING"
```

```python
# ApplicationDiscoveryStatusType definition

ApplicationDiscoveryStatusType = Literal[
    "DELETING",
    "REFRESH_FAILED",
    "REGISTERING",
    "REGISTRATION_FAILED",
    "SUCCESS",
]
```
## ApplicationStatusType

```python
# ApplicationStatusType usage example

from types_aiobotocore_ssm_sap.literals import ApplicationStatusType

def get_value() -> ApplicationStatusType:
    return "ACTIVATED"
```

```python
# ApplicationStatusType definition

ApplicationStatusType = Literal[
    "ACTIVATED",
    "DELETING",
    "FAILED",
    "REGISTERING",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "UNKNOWN",
]
```
## ApplicationTypeType

```python
# ApplicationTypeType usage example

from types_aiobotocore_ssm_sap.literals import ApplicationTypeType

def get_value() -> ApplicationTypeType:
    return "HANA"
```

```python
# ApplicationTypeType definition

ApplicationTypeType = Literal[
    "HANA",
]
```
## BackintModeType

```python
# BackintModeType usage example

from types_aiobotocore_ssm_sap.literals import BackintModeType

def get_value() -> BackintModeType:
    return "AWSBackup"
```

```python
# BackintModeType definition

BackintModeType = Literal[
    "AWSBackup",
]
```
## ClusterStatusType

```python
# ClusterStatusType usage example

from types_aiobotocore_ssm_sap.literals import ClusterStatusType

def get_value() -> ClusterStatusType:
    return "MAINTENANCE"
```

```python
# ClusterStatusType definition

ClusterStatusType = Literal[
    "MAINTENANCE",
    "NONE",
    "OFFLINE",
    "ONLINE",
    "STANDBY",
]
```
## ComponentStatusType

```python
# ComponentStatusType usage example

from types_aiobotocore_ssm_sap.literals import ComponentStatusType

def get_value() -> ComponentStatusType:
    return "ACTIVATED"
```

```python
# ComponentStatusType definition

ComponentStatusType = Literal[
    "ACTIVATED",
    "RUNNING",
    "RUNNING_WITH_ERROR",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "UNDEFINED",
]
```
## ComponentTypeType

```python
# ComponentTypeType usage example

from types_aiobotocore_ssm_sap.literals import ComponentTypeType

def get_value() -> ComponentTypeType:
    return "HANA"
```

```python
# ComponentTypeType definition

ComponentTypeType = Literal[
    "HANA",
    "HANA_NODE",
]
```
## CredentialTypeType

```python
# CredentialTypeType usage example

from types_aiobotocore_ssm_sap.literals import CredentialTypeType

def get_value() -> CredentialTypeType:
    return "ADMIN"
```

```python
# CredentialTypeType definition

CredentialTypeType = Literal[
    "ADMIN",
]
```
## DatabaseStatusType

```python
# DatabaseStatusType usage example

from types_aiobotocore_ssm_sap.literals import DatabaseStatusType

def get_value() -> DatabaseStatusType:
    return "ERROR"
```

```python
# DatabaseStatusType definition

DatabaseStatusType = Literal[
    "ERROR",
    "RUNNING",
    "STARTING",
    "STOPPED",
    "UNKNOWN",
    "WARNING",
]
```
## DatabaseTypeType

```python
# DatabaseTypeType usage example

from types_aiobotocore_ssm_sap.literals import DatabaseTypeType

def get_value() -> DatabaseTypeType:
    return "SYSTEM"
```

```python
# DatabaseTypeType definition

DatabaseTypeType = Literal[
    "SYSTEM",
    "TENANT",
]
```
## FilterOperatorType

```python
# FilterOperatorType usage example

from types_aiobotocore_ssm_sap.literals import FilterOperatorType

def get_value() -> FilterOperatorType:
    return "Equals"
```

```python
# FilterOperatorType definition

FilterOperatorType = Literal[
    "Equals",
    "GreaterThanOrEquals",
    "LessThanOrEquals",
]
```
## HostRoleType

```python
# HostRoleType usage example

from types_aiobotocore_ssm_sap.literals import HostRoleType

def get_value() -> HostRoleType:
    return "LEADER"
```

```python
# HostRoleType definition

HostRoleType = Literal[
    "LEADER",
    "STANDBY",
    "UNKNOWN",
    "WORKER",
]
```
## ListApplicationsPaginatorName

```python
# ListApplicationsPaginatorName usage example

from types_aiobotocore_ssm_sap.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python
# ListApplicationsPaginatorName definition

ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListComponentsPaginatorName

```python
# ListComponentsPaginatorName usage example

from types_aiobotocore_ssm_sap.literals import ListComponentsPaginatorName

def get_value() -> ListComponentsPaginatorName:
    return "list_components"
```

```python
# ListComponentsPaginatorName definition

ListComponentsPaginatorName = Literal[
    "list_components",
]
```
## ListDatabasesPaginatorName

```python
# ListDatabasesPaginatorName usage example

from types_aiobotocore_ssm_sap.literals import ListDatabasesPaginatorName

def get_value() -> ListDatabasesPaginatorName:
    return "list_databases"
```

```python
# ListDatabasesPaginatorName definition

ListDatabasesPaginatorName = Literal[
    "list_databases",
]
```
## ListOperationsPaginatorName

```python
# ListOperationsPaginatorName usage example

from types_aiobotocore_ssm_sap.literals import ListOperationsPaginatorName

def get_value() -> ListOperationsPaginatorName:
    return "list_operations"
```

```python
# ListOperationsPaginatorName definition

ListOperationsPaginatorName = Literal[
    "list_operations",
]
```
## OperationModeType

```python
# OperationModeType usage example

from types_aiobotocore_ssm_sap.literals import OperationModeType

def get_value() -> OperationModeType:
    return "DELTA_DATASHIPPING"
```

```python
# OperationModeType definition

OperationModeType = Literal[
    "DELTA_DATASHIPPING",
    "LOGREPLAY",
    "LOGREPLAY_READACCESS",
    "NONE",
    "PRIMARY",
]
```
## OperationStatusType

```python
# OperationStatusType usage example

from types_aiobotocore_ssm_sap.literals import OperationStatusType

def get_value() -> OperationStatusType:
    return "ERROR"
```

```python
# OperationStatusType definition

OperationStatusType = Literal[
    "ERROR",
    "INPROGRESS",
    "SUCCESS",
]
```
## PermissionActionTypeType

```python
# PermissionActionTypeType usage example

from types_aiobotocore_ssm_sap.literals import PermissionActionTypeType

def get_value() -> PermissionActionTypeType:
    return "RESTORE"
```

```python
# PermissionActionTypeType definition

PermissionActionTypeType = Literal[
    "RESTORE",
]
```
## ReplicationModeType

```python
# ReplicationModeType usage example

from types_aiobotocore_ssm_sap.literals import ReplicationModeType

def get_value() -> ReplicationModeType:
    return "ASYNC"
```

```python
# ReplicationModeType definition

ReplicationModeType = Literal[
    "ASYNC",
    "NONE",
    "PRIMARY",
    "SYNC",
    "SYNCMEM",
]
```
## SsmSapServiceName

```python
# SsmSapServiceName usage example

from types_aiobotocore_ssm_sap.literals import SsmSapServiceName

def get_value() -> SsmSapServiceName:
    return "ssm-sap"
```

```python
# SsmSapServiceName definition

SsmSapServiceName = Literal[
    "ssm-sap",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_ssm_sap.literals import ServiceName

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

from types_aiobotocore_ssm_sap.literals import ResourceServiceName

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

from types_aiobotocore_ssm_sap.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_applications"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_applications",
    "list_components",
    "list_databases",
    "list_operations",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_ssm_sap.literals import RegionName

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
