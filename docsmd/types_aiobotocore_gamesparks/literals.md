# Literals

> [Index](../README.md) > [GameSparks](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [GameSparks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
    type annotations stubs module [types-aiobotocore-gamesparks](https://pypi.org/project/types-aiobotocore-gamesparks/).

## DeploymentActionType

```python
# DeploymentActionType usage example

from types_aiobotocore_gamesparks.literals import DeploymentActionType

def get_value() -> DeploymentActionType:
    return "DEPLOY"
```

```python
# DeploymentActionType definition

DeploymentActionType = Literal[
    "DEPLOY",
    "UNDEPLOY",
]
```
## DeploymentStateType

```python
# DeploymentStateType usage example

from types_aiobotocore_gamesparks.literals import DeploymentStateType

def get_value() -> DeploymentStateType:
    return "COMPLETED"
```

```python
# DeploymentStateType definition

DeploymentStateType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "PENDING",
]
```
## GameStateType

```python
# GameStateType usage example

from types_aiobotocore_gamesparks.literals import GameStateType

def get_value() -> GameStateType:
    return "ACTIVE"
```

```python
# GameStateType definition

GameStateType = Literal[
    "ACTIVE",
    "DELETING",
]
```
## GeneratedCodeJobStateType

```python
# GeneratedCodeJobStateType usage example

from types_aiobotocore_gamesparks.literals import GeneratedCodeJobStateType

def get_value() -> GeneratedCodeJobStateType:
    return "COMPLETED"
```

```python
# GeneratedCodeJobStateType definition

GeneratedCodeJobStateType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "PENDING",
]
```
## ListExtensionVersionsPaginatorName

```python
# ListExtensionVersionsPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListExtensionVersionsPaginatorName

def get_value() -> ListExtensionVersionsPaginatorName:
    return "list_extension_versions"
```

```python
# ListExtensionVersionsPaginatorName definition

ListExtensionVersionsPaginatorName = Literal[
    "list_extension_versions",
]
```
## ListExtensionsPaginatorName

```python
# ListExtensionsPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListExtensionsPaginatorName

def get_value() -> ListExtensionsPaginatorName:
    return "list_extensions"
```

```python
# ListExtensionsPaginatorName definition

ListExtensionsPaginatorName = Literal[
    "list_extensions",
]
```
## ListGamesPaginatorName

```python
# ListGamesPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListGamesPaginatorName

def get_value() -> ListGamesPaginatorName:
    return "list_games"
```

```python
# ListGamesPaginatorName definition

ListGamesPaginatorName = Literal[
    "list_games",
]
```
## ListGeneratedCodeJobsPaginatorName

```python
# ListGeneratedCodeJobsPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListGeneratedCodeJobsPaginatorName

def get_value() -> ListGeneratedCodeJobsPaginatorName:
    return "list_generated_code_jobs"
```

```python
# ListGeneratedCodeJobsPaginatorName definition

ListGeneratedCodeJobsPaginatorName = Literal[
    "list_generated_code_jobs",
]
```
## ListSnapshotsPaginatorName

```python
# ListSnapshotsPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListSnapshotsPaginatorName

def get_value() -> ListSnapshotsPaginatorName:
    return "list_snapshots"
```

```python
# ListSnapshotsPaginatorName definition

ListSnapshotsPaginatorName = Literal[
    "list_snapshots",
]
```
## ListStageDeploymentsPaginatorName

```python
# ListStageDeploymentsPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListStageDeploymentsPaginatorName

def get_value() -> ListStageDeploymentsPaginatorName:
    return "list_stage_deployments"
```

```python
# ListStageDeploymentsPaginatorName definition

ListStageDeploymentsPaginatorName = Literal[
    "list_stage_deployments",
]
```
## ListStagesPaginatorName

```python
# ListStagesPaginatorName usage example

from types_aiobotocore_gamesparks.literals import ListStagesPaginatorName

def get_value() -> ListStagesPaginatorName:
    return "list_stages"
```

```python
# ListStagesPaginatorName definition

ListStagesPaginatorName = Literal[
    "list_stages",
]
```
## OperationType

```python
# OperationType usage example

from types_aiobotocore_gamesparks.literals import OperationType

def get_value() -> OperationType:
    return "ADD"
```

```python
# OperationType definition

OperationType = Literal[
    "ADD",
    "REMOVE",
    "REPLACE",
]
```
## ResultCodeType

```python
# ResultCodeType usage example

from types_aiobotocore_gamesparks.literals import ResultCodeType

def get_value() -> ResultCodeType:
    return "INVALID_ROLE_FAILURE"
```

```python
# ResultCodeType definition

ResultCodeType = Literal[
    "INVALID_ROLE_FAILURE",
    "SUCCESS",
    "UNSPECIFIED_FAILURE",
]
```
## StageStateType

```python
# StageStateType usage example

from types_aiobotocore_gamesparks.literals import StageStateType

def get_value() -> StageStateType:
    return "ACTIVE"
```

```python
# StageStateType definition

StageStateType = Literal[
    "ACTIVE",
    "DELETING",
]
```
## GameSparksServiceName

```python
# GameSparksServiceName usage example

from types_aiobotocore_gamesparks.literals import GameSparksServiceName

def get_value() -> GameSparksServiceName:
    return "gamesparks"
```

```python
# GameSparksServiceName definition

GameSparksServiceName = Literal[
    "gamesparks",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_gamesparks.literals import ServiceName

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

from types_aiobotocore_gamesparks.literals import ResourceServiceName

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

from types_aiobotocore_gamesparks.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_extension_versions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_extension_versions",
    "list_extensions",
    "list_games",
    "list_generated_code_jobs",
    "list_snapshots",
    "list_stage_deployments",
    "list_stages",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_gamesparks.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "us-east-1",
]
```
