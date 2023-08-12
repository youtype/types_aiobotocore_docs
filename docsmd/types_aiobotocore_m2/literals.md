# Literals

> [Index](../README.md) > [MainframeModernization](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## ApplicationDeploymentLifecycleType

```python
# ApplicationDeploymentLifecycleType usage example

from types_aiobotocore_m2.literals import ApplicationDeploymentLifecycleType

def get_value() -> ApplicationDeploymentLifecycleType:
    return "Deployed"
```

```python
# ApplicationDeploymentLifecycleType definition

ApplicationDeploymentLifecycleType = Literal[
    "Deployed",
    "Deploying",
]
```
## ApplicationLifecycleType

```python
# ApplicationLifecycleType usage example

from types_aiobotocore_m2.literals import ApplicationLifecycleType

def get_value() -> ApplicationLifecycleType:
    return "Available"
```

```python
# ApplicationLifecycleType definition

ApplicationLifecycleType = Literal[
    "Available",
    "Created",
    "Creating",
    "Deleting",
    "Deleting From Environment",
    "Failed",
    "Ready",
    "Running",
    "Starting",
    "Stopped",
    "Stopping",
]
```
## ApplicationVersionLifecycleType

```python
# ApplicationVersionLifecycleType usage example

from types_aiobotocore_m2.literals import ApplicationVersionLifecycleType

def get_value() -> ApplicationVersionLifecycleType:
    return "Available"
```

```python
# ApplicationVersionLifecycleType definition

ApplicationVersionLifecycleType = Literal[
    "Available",
    "Creating",
    "Failed",
]
```
## BatchJobExecutionStatusType

```python
# BatchJobExecutionStatusType usage example

from types_aiobotocore_m2.literals import BatchJobExecutionStatusType

def get_value() -> BatchJobExecutionStatusType:
    return "Cancelled"
```

```python
# BatchJobExecutionStatusType definition

BatchJobExecutionStatusType = Literal[
    "Cancelled",
    "Cancelling",
    "Dispatching",
    "Failed",
    "Holding",
    "Running",
    "Submitting",
    "Succeeded",
    "Succeeded With Warning",
]
```
## BatchJobTypeType

```python
# BatchJobTypeType usage example

from types_aiobotocore_m2.literals import BatchJobTypeType

def get_value() -> BatchJobTypeType:
    return "JES2"
```

```python
# BatchJobTypeType definition

BatchJobTypeType = Literal[
    "JES2",
    "JES3",
    "VSE",
]
```
## DataSetTaskLifecycleType

```python
# DataSetTaskLifecycleType usage example

from types_aiobotocore_m2.literals import DataSetTaskLifecycleType

def get_value() -> DataSetTaskLifecycleType:
    return "Completed"
```

```python
# DataSetTaskLifecycleType definition

DataSetTaskLifecycleType = Literal[
    "Completed",
    "Creating",
    "Running",
]
```
## DeploymentLifecycleType

```python
# DeploymentLifecycleType usage example

from types_aiobotocore_m2.literals import DeploymentLifecycleType

def get_value() -> DeploymentLifecycleType:
    return "Deploying"
```

```python
# DeploymentLifecycleType definition

DeploymentLifecycleType = Literal[
    "Deploying",
    "Failed",
    "Succeeded",
]
```
## EngineTypeType

```python
# EngineTypeType usage example

from types_aiobotocore_m2.literals import EngineTypeType

def get_value() -> EngineTypeType:
    return "bluage"
```

```python
# EngineTypeType definition

EngineTypeType = Literal[
    "bluage",
    "microfocus",
]
```
## EnvironmentLifecycleType

```python
# EnvironmentLifecycleType usage example

from types_aiobotocore_m2.literals import EnvironmentLifecycleType

def get_value() -> EnvironmentLifecycleType:
    return "Available"
```

```python
# EnvironmentLifecycleType definition

EnvironmentLifecycleType = Literal[
    "Available",
    "Creating",
    "Deleting",
    "Failed",
    "Updating",
]
```
## ListApplicationVersionsPaginatorName

```python
# ListApplicationVersionsPaginatorName usage example

from types_aiobotocore_m2.literals import ListApplicationVersionsPaginatorName

def get_value() -> ListApplicationVersionsPaginatorName:
    return "list_application_versions"
```

```python
# ListApplicationVersionsPaginatorName definition

ListApplicationVersionsPaginatorName = Literal[
    "list_application_versions",
]
```
## ListApplicationsPaginatorName

```python
# ListApplicationsPaginatorName usage example

from types_aiobotocore_m2.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python
# ListApplicationsPaginatorName definition

ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListBatchJobDefinitionsPaginatorName

```python
# ListBatchJobDefinitionsPaginatorName usage example

from types_aiobotocore_m2.literals import ListBatchJobDefinitionsPaginatorName

def get_value() -> ListBatchJobDefinitionsPaginatorName:
    return "list_batch_job_definitions"
```

```python
# ListBatchJobDefinitionsPaginatorName definition

ListBatchJobDefinitionsPaginatorName = Literal[
    "list_batch_job_definitions",
]
```
## ListBatchJobExecutionsPaginatorName

```python
# ListBatchJobExecutionsPaginatorName usage example

from types_aiobotocore_m2.literals import ListBatchJobExecutionsPaginatorName

def get_value() -> ListBatchJobExecutionsPaginatorName:
    return "list_batch_job_executions"
```

```python
# ListBatchJobExecutionsPaginatorName definition

ListBatchJobExecutionsPaginatorName = Literal[
    "list_batch_job_executions",
]
```
## ListDataSetImportHistoryPaginatorName

```python
# ListDataSetImportHistoryPaginatorName usage example

from types_aiobotocore_m2.literals import ListDataSetImportHistoryPaginatorName

def get_value() -> ListDataSetImportHistoryPaginatorName:
    return "list_data_set_import_history"
```

```python
# ListDataSetImportHistoryPaginatorName definition

ListDataSetImportHistoryPaginatorName = Literal[
    "list_data_set_import_history",
]
```
## ListDataSetsPaginatorName

```python
# ListDataSetsPaginatorName usage example

from types_aiobotocore_m2.literals import ListDataSetsPaginatorName

def get_value() -> ListDataSetsPaginatorName:
    return "list_data_sets"
```

```python
# ListDataSetsPaginatorName definition

ListDataSetsPaginatorName = Literal[
    "list_data_sets",
]
```
## ListDeploymentsPaginatorName

```python
# ListDeploymentsPaginatorName usage example

from types_aiobotocore_m2.literals import ListDeploymentsPaginatorName

def get_value() -> ListDeploymentsPaginatorName:
    return "list_deployments"
```

```python
# ListDeploymentsPaginatorName definition

ListDeploymentsPaginatorName = Literal[
    "list_deployments",
]
```
## ListEngineVersionsPaginatorName

```python
# ListEngineVersionsPaginatorName usage example

from types_aiobotocore_m2.literals import ListEngineVersionsPaginatorName

def get_value() -> ListEngineVersionsPaginatorName:
    return "list_engine_versions"
```

```python
# ListEngineVersionsPaginatorName definition

ListEngineVersionsPaginatorName = Literal[
    "list_engine_versions",
]
```
## ListEnvironmentsPaginatorName

```python
# ListEnvironmentsPaginatorName usage example

from types_aiobotocore_m2.literals import ListEnvironmentsPaginatorName

def get_value() -> ListEnvironmentsPaginatorName:
    return "list_environments"
```

```python
# ListEnvironmentsPaginatorName definition

ListEnvironmentsPaginatorName = Literal[
    "list_environments",
]
```
## MainframeModernizationServiceName

```python
# MainframeModernizationServiceName usage example

from types_aiobotocore_m2.literals import MainframeModernizationServiceName

def get_value() -> MainframeModernizationServiceName:
    return "m2"
```

```python
# MainframeModernizationServiceName definition

MainframeModernizationServiceName = Literal[
    "m2",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_m2.literals import ServiceName

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

from types_aiobotocore_m2.literals import ResourceServiceName

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

from types_aiobotocore_m2.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_application_versions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_application_versions",
    "list_applications",
    "list_batch_job_definitions",
    "list_batch_job_executions",
    "list_data_set_import_history",
    "list_data_sets",
    "list_deployments",
    "list_engine_versions",
    "list_environments",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_m2.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
