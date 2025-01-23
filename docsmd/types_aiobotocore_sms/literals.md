# Literals

> [Index](../README.md) > [SMS](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#sms)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## AppLaunchConfigurationStatusType

```python
# AppLaunchConfigurationStatusType usage example

from types_aiobotocore_sms.literals import AppLaunchConfigurationStatusType

def get_value() -> AppLaunchConfigurationStatusType:
    return "CONFIGURED"
```

```python
# AppLaunchConfigurationStatusType definition

AppLaunchConfigurationStatusType = Literal[
    "CONFIGURED",
    "NOT_CONFIGURED",
]
```
## AppLaunchStatusType

```python
# AppLaunchStatusType usage example

from types_aiobotocore_sms.literals import AppLaunchStatusType

def get_value() -> AppLaunchStatusType:
    return "CONFIGURATION_INVALID"
```

```python
# AppLaunchStatusType definition

AppLaunchStatusType = Literal[
    "CONFIGURATION_IN_PROGRESS",
    "CONFIGURATION_INVALID",
    "DELTA_LAUNCH_FAILED",
    "DELTA_LAUNCH_IN_PROGRESS",
    "LAUNCH_FAILED",
    "LAUNCH_IN_PROGRESS",
    "LAUNCH_PENDING",
    "LAUNCHED",
    "PARTIALLY_LAUNCHED",
    "READY_FOR_CONFIGURATION",
    "READY_FOR_LAUNCH",
    "TERMINATE_FAILED",
    "TERMINATE_IN_PROGRESS",
    "TERMINATED",
    "VALIDATION_IN_PROGRESS",
]
```
## AppReplicationConfigurationStatusType

```python
# AppReplicationConfigurationStatusType usage example

from types_aiobotocore_sms.literals import AppReplicationConfigurationStatusType

def get_value() -> AppReplicationConfigurationStatusType:
    return "CONFIGURED"
```

```python
# AppReplicationConfigurationStatusType definition

AppReplicationConfigurationStatusType = Literal[
    "CONFIGURED",
    "NOT_CONFIGURED",
]
```
## AppReplicationStatusType

```python
# AppReplicationStatusType usage example

from types_aiobotocore_sms.literals import AppReplicationStatusType

def get_value() -> AppReplicationStatusType:
    return "CONFIGURATION_INVALID"
```

```python
# AppReplicationStatusType definition

AppReplicationStatusType = Literal[
    "CONFIGURATION_IN_PROGRESS",
    "CONFIGURATION_INVALID",
    "DELTA_REPLICATED",
    "DELTA_REPLICATION_FAILED",
    "DELTA_REPLICATION_IN_PROGRESS",
    "PARTIALLY_REPLICATED",
    "READY_FOR_CONFIGURATION",
    "READY_FOR_REPLICATION",
    "REPLICATED",
    "REPLICATION_FAILED",
    "REPLICATION_IN_PROGRESS",
    "REPLICATION_PENDING",
    "REPLICATION_STOP_FAILED",
    "REPLICATION_STOPPED",
    "REPLICATION_STOPPING",
    "VALIDATION_IN_PROGRESS",
]
```
## AppStatusType

```python
# AppStatusType usage example

from types_aiobotocore_sms.literals import AppStatusType

def get_value() -> AppStatusType:
    return "ACTIVE"
```

```python
# AppStatusType definition

AppStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "UPDATING",
]
```
## AppValidationStrategyType

```python
# AppValidationStrategyType usage example

from types_aiobotocore_sms.literals import AppValidationStrategyType

def get_value() -> AppValidationStrategyType:
    return "SSM"
```

```python
# AppValidationStrategyType definition

AppValidationStrategyType = Literal[
    "SSM",
]
```
## ConnectorCapabilityType

```python
# ConnectorCapabilityType usage example

from types_aiobotocore_sms.literals import ConnectorCapabilityType

def get_value() -> ConnectorCapabilityType:
    return "HYPERV-MANAGER"
```

```python
# ConnectorCapabilityType definition

ConnectorCapabilityType = Literal[
    "HYPERV-MANAGER",
    "SCVMM",
    "SMS_OPTIMIZED",
    "SNAPSHOT_BATCHING",
    "VSPHERE",
]
```
## ConnectorStatusType

```python
# ConnectorStatusType usage example

from types_aiobotocore_sms.literals import ConnectorStatusType

def get_value() -> ConnectorStatusType:
    return "HEALTHY"
```

```python
# ConnectorStatusType definition

ConnectorStatusType = Literal[
    "HEALTHY",
    "UNHEALTHY",
]
```
## GetConnectorsPaginatorName

```python
# GetConnectorsPaginatorName usage example

from types_aiobotocore_sms.literals import GetConnectorsPaginatorName

def get_value() -> GetConnectorsPaginatorName:
    return "get_connectors"
```

```python
# GetConnectorsPaginatorName definition

GetConnectorsPaginatorName = Literal[
    "get_connectors",
]
```
## GetReplicationJobsPaginatorName

```python
# GetReplicationJobsPaginatorName usage example

from types_aiobotocore_sms.literals import GetReplicationJobsPaginatorName

def get_value() -> GetReplicationJobsPaginatorName:
    return "get_replication_jobs"
```

```python
# GetReplicationJobsPaginatorName definition

GetReplicationJobsPaginatorName = Literal[
    "get_replication_jobs",
]
```
## GetReplicationRunsPaginatorName

```python
# GetReplicationRunsPaginatorName usage example

from types_aiobotocore_sms.literals import GetReplicationRunsPaginatorName

def get_value() -> GetReplicationRunsPaginatorName:
    return "get_replication_runs"
```

```python
# GetReplicationRunsPaginatorName definition

GetReplicationRunsPaginatorName = Literal[
    "get_replication_runs",
]
```
## GetServersPaginatorName

```python
# GetServersPaginatorName usage example

from types_aiobotocore_sms.literals import GetServersPaginatorName

def get_value() -> GetServersPaginatorName:
    return "get_servers"
```

```python
# GetServersPaginatorName definition

GetServersPaginatorName = Literal[
    "get_servers",
]
```
## LicenseTypeType

```python
# LicenseTypeType usage example

from types_aiobotocore_sms.literals import LicenseTypeType

def get_value() -> LicenseTypeType:
    return "AWS"
```

```python
# LicenseTypeType definition

LicenseTypeType = Literal[
    "AWS",
    "BYOL",
]
```
## ListAppsPaginatorName

```python
# ListAppsPaginatorName usage example

from types_aiobotocore_sms.literals import ListAppsPaginatorName

def get_value() -> ListAppsPaginatorName:
    return "list_apps"
```

```python
# ListAppsPaginatorName definition

ListAppsPaginatorName = Literal[
    "list_apps",
]
```
## OutputFormatType

```python
# OutputFormatType usage example

from types_aiobotocore_sms.literals import OutputFormatType

def get_value() -> OutputFormatType:
    return "JSON"
```

```python
# OutputFormatType definition

OutputFormatType = Literal[
    "JSON",
    "YAML",
]
```
## ReplicationJobStateType

```python
# ReplicationJobStateType usage example

from types_aiobotocore_sms.literals import ReplicationJobStateType

def get_value() -> ReplicationJobStateType:
    return "ACTIVE"
```

```python
# ReplicationJobStateType definition

ReplicationJobStateType = Literal[
    "ACTIVE",
    "COMPLETED",
    "DELETED",
    "DELETING",
    "FAILED",
    "FAILING",
    "PAUSED_ON_FAILURE",
    "PENDING",
]
```
## ReplicationRunStateType

```python
# ReplicationRunStateType usage example

from types_aiobotocore_sms.literals import ReplicationRunStateType

def get_value() -> ReplicationRunStateType:
    return "ACTIVE"
```

```python
# ReplicationRunStateType definition

ReplicationRunStateType = Literal[
    "ACTIVE",
    "COMPLETED",
    "DELETED",
    "DELETING",
    "FAILED",
    "MISSED",
    "PENDING",
]
```
## ReplicationRunTypeType

```python
# ReplicationRunTypeType usage example

from types_aiobotocore_sms.literals import ReplicationRunTypeType

def get_value() -> ReplicationRunTypeType:
    return "AUTOMATIC"
```

```python
# ReplicationRunTypeType definition

ReplicationRunTypeType = Literal[
    "AUTOMATIC",
    "ON_DEMAND",
]
```
## ScriptTypeType

```python
# ScriptTypeType usage example

from types_aiobotocore_sms.literals import ScriptTypeType

def get_value() -> ScriptTypeType:
    return "POWERSHELL_SCRIPT"
```

```python
# ScriptTypeType definition

ScriptTypeType = Literal[
    "POWERSHELL_SCRIPT",
    "SHELL_SCRIPT",
]
```
## ServerCatalogStatusType

```python
# ServerCatalogStatusType usage example

from types_aiobotocore_sms.literals import ServerCatalogStatusType

def get_value() -> ServerCatalogStatusType:
    return "AVAILABLE"
```

```python
# ServerCatalogStatusType definition

ServerCatalogStatusType = Literal[
    "AVAILABLE",
    "DELETED",
    "EXPIRED",
    "IMPORTING",
    "NOT_IMPORTED",
]
```
## ServerTypeType

```python
# ServerTypeType usage example

from types_aiobotocore_sms.literals import ServerTypeType

def get_value() -> ServerTypeType:
    return "VIRTUAL_MACHINE"
```

```python
# ServerTypeType definition

ServerTypeType = Literal[
    "VIRTUAL_MACHINE",
]
```
## ServerValidationStrategyType

```python
# ServerValidationStrategyType usage example

from types_aiobotocore_sms.literals import ServerValidationStrategyType

def get_value() -> ServerValidationStrategyType:
    return "USERDATA"
```

```python
# ServerValidationStrategyType definition

ServerValidationStrategyType = Literal[
    "USERDATA",
]
```
## ValidationStatusType

```python
# ValidationStatusType usage example

from types_aiobotocore_sms.literals import ValidationStatusType

def get_value() -> ValidationStatusType:
    return "FAILED"
```

```python
# ValidationStatusType definition

ValidationStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "PENDING",
    "READY_FOR_VALIDATION",
    "SUCCEEDED",
]
```
## VmManagerTypeType

```python
# VmManagerTypeType usage example

from types_aiobotocore_sms.literals import VmManagerTypeType

def get_value() -> VmManagerTypeType:
    return "HYPERV-MANAGER"
```

```python
# VmManagerTypeType definition

VmManagerTypeType = Literal[
    "HYPERV-MANAGER",
    "SCVMM",
    "VSPHERE",
]
```
## SMSServiceName

```python
# SMSServiceName usage example

from types_aiobotocore_sms.literals import SMSServiceName

def get_value() -> SMSServiceName:
    return "sms"
```

```python
# SMSServiceName definition

SMSServiceName = Literal[
    "sms",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_sms.literals import ServiceName

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

from types_aiobotocore_sms.literals import ResourceServiceName

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

from types_aiobotocore_sms.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_connectors"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_connectors",
    "get_replication_jobs",
    "get_replication_runs",
    "get_servers",
    "list_apps",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_sms.literals import RegionName

def get_value() -> RegionName:
    return "us-west-2"
```

```python
# RegionName definition

RegionName = Literal[
    "us-west-2",
]
```
