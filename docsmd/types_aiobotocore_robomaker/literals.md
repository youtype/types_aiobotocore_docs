# Literals

> [Index](../README.md) > [RoboMaker](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## ArchitectureType

```python
# ArchitectureType usage example

from types_aiobotocore_robomaker.literals import ArchitectureType

def get_value() -> ArchitectureType:
    return "ARM64"
```

```python
# ArchitectureType definition

ArchitectureType = Literal[
    "ARM64",
    "ARMHF",
    "X86_64",
]
```
## ComputeTypeType

```python
# ComputeTypeType usage example

from types_aiobotocore_robomaker.literals import ComputeTypeType

def get_value() -> ComputeTypeType:
    return "CPU"
```

```python
# ComputeTypeType definition

ComputeTypeType = Literal[
    "CPU",
    "GPU_AND_CPU",
]
```
## DataSourceTypeType

```python
# DataSourceTypeType usage example

from types_aiobotocore_robomaker.literals import DataSourceTypeType

def get_value() -> DataSourceTypeType:
    return "Archive"
```

```python
# DataSourceTypeType definition

DataSourceTypeType = Literal[
    "Archive",
    "File",
    "Prefix",
]
```
## DeploymentJobErrorCodeType

```python
# DeploymentJobErrorCodeType usage example

from types_aiobotocore_robomaker.literals import DeploymentJobErrorCodeType

def get_value() -> DeploymentJobErrorCodeType:
    return "BadLambdaAssociated"
```

```python
# DeploymentJobErrorCodeType definition

DeploymentJobErrorCodeType = Literal[
    "BadLambdaAssociated",
    "BadPermissionError",
    "DeploymentFleetDoesNotExist",
    "DownloadConditionFailed",
    "EnvironmentSetupError",
    "EtagMismatch",
    "ExtractingBundleFailure",
    "FailureThresholdBreached",
    "FleetDeploymentTimeout",
    "GreengrassDeploymentFailed",
    "GreengrassGroupVersionDoesNotExist",
    "InternalServerError",
    "InvalidGreengrassGroup",
    "LambdaDeleted",
    "MissingRobotApplicationArchitecture",
    "MissingRobotArchitecture",
    "MissingRobotDeploymentResource",
    "PostLaunchFileFailure",
    "PreLaunchFileFailure",
    "ResourceNotFound",
    "RobotAgentConnectionTimeout",
    "RobotApplicationDoesNotExist",
    "RobotDeploymentAborted",
    "RobotDeploymentNoResponse",
]
```
## DeploymentStatusType

```python
# DeploymentStatusType usage example

from types_aiobotocore_robomaker.literals import DeploymentStatusType

def get_value() -> DeploymentStatusType:
    return "Canceled"
```

```python
# DeploymentStatusType definition

DeploymentStatusType = Literal[
    "Canceled",
    "Failed",
    "InProgress",
    "Pending",
    "Preparing",
    "Succeeded",
]
```
## ExitBehaviorType

```python
# ExitBehaviorType usage example

from types_aiobotocore_robomaker.literals import ExitBehaviorType

def get_value() -> ExitBehaviorType:
    return "FAIL"
```

```python
# ExitBehaviorType definition

ExitBehaviorType = Literal[
    "FAIL",
    "RESTART",
]
```
## FailureBehaviorType

```python
# FailureBehaviorType usage example

from types_aiobotocore_robomaker.literals import FailureBehaviorType

def get_value() -> FailureBehaviorType:
    return "Continue"
```

```python
# FailureBehaviorType definition

FailureBehaviorType = Literal[
    "Continue",
    "Fail",
]
```
## ListDeploymentJobsPaginatorName

```python
# ListDeploymentJobsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListDeploymentJobsPaginatorName

def get_value() -> ListDeploymentJobsPaginatorName:
    return "list_deployment_jobs"
```

```python
# ListDeploymentJobsPaginatorName definition

ListDeploymentJobsPaginatorName = Literal[
    "list_deployment_jobs",
]
```
## ListFleetsPaginatorName

```python
# ListFleetsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListFleetsPaginatorName

def get_value() -> ListFleetsPaginatorName:
    return "list_fleets"
```

```python
# ListFleetsPaginatorName definition

ListFleetsPaginatorName = Literal[
    "list_fleets",
]
```
## ListRobotApplicationsPaginatorName

```python
# ListRobotApplicationsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListRobotApplicationsPaginatorName

def get_value() -> ListRobotApplicationsPaginatorName:
    return "list_robot_applications"
```

```python
# ListRobotApplicationsPaginatorName definition

ListRobotApplicationsPaginatorName = Literal[
    "list_robot_applications",
]
```
## ListRobotsPaginatorName

```python
# ListRobotsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListRobotsPaginatorName

def get_value() -> ListRobotsPaginatorName:
    return "list_robots"
```

```python
# ListRobotsPaginatorName definition

ListRobotsPaginatorName = Literal[
    "list_robots",
]
```
## ListSimulationApplicationsPaginatorName

```python
# ListSimulationApplicationsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListSimulationApplicationsPaginatorName

def get_value() -> ListSimulationApplicationsPaginatorName:
    return "list_simulation_applications"
```

```python
# ListSimulationApplicationsPaginatorName definition

ListSimulationApplicationsPaginatorName = Literal[
    "list_simulation_applications",
]
```
## ListSimulationJobBatchesPaginatorName

```python
# ListSimulationJobBatchesPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListSimulationJobBatchesPaginatorName

def get_value() -> ListSimulationJobBatchesPaginatorName:
    return "list_simulation_job_batches"
```

```python
# ListSimulationJobBatchesPaginatorName definition

ListSimulationJobBatchesPaginatorName = Literal[
    "list_simulation_job_batches",
]
```
## ListSimulationJobsPaginatorName

```python
# ListSimulationJobsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListSimulationJobsPaginatorName

def get_value() -> ListSimulationJobsPaginatorName:
    return "list_simulation_jobs"
```

```python
# ListSimulationJobsPaginatorName definition

ListSimulationJobsPaginatorName = Literal[
    "list_simulation_jobs",
]
```
## ListWorldExportJobsPaginatorName

```python
# ListWorldExportJobsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListWorldExportJobsPaginatorName

def get_value() -> ListWorldExportJobsPaginatorName:
    return "list_world_export_jobs"
```

```python
# ListWorldExportJobsPaginatorName definition

ListWorldExportJobsPaginatorName = Literal[
    "list_world_export_jobs",
]
```
## ListWorldGenerationJobsPaginatorName

```python
# ListWorldGenerationJobsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListWorldGenerationJobsPaginatorName

def get_value() -> ListWorldGenerationJobsPaginatorName:
    return "list_world_generation_jobs"
```

```python
# ListWorldGenerationJobsPaginatorName definition

ListWorldGenerationJobsPaginatorName = Literal[
    "list_world_generation_jobs",
]
```
## ListWorldTemplatesPaginatorName

```python
# ListWorldTemplatesPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListWorldTemplatesPaginatorName

def get_value() -> ListWorldTemplatesPaginatorName:
    return "list_world_templates"
```

```python
# ListWorldTemplatesPaginatorName definition

ListWorldTemplatesPaginatorName = Literal[
    "list_world_templates",
]
```
## ListWorldsPaginatorName

```python
# ListWorldsPaginatorName usage example

from types_aiobotocore_robomaker.literals import ListWorldsPaginatorName

def get_value() -> ListWorldsPaginatorName:
    return "list_worlds"
```

```python
# ListWorldsPaginatorName definition

ListWorldsPaginatorName = Literal[
    "list_worlds",
]
```
## RenderingEngineTypeType

```python
# RenderingEngineTypeType usage example

from types_aiobotocore_robomaker.literals import RenderingEngineTypeType

def get_value() -> RenderingEngineTypeType:
    return "OGRE"
```

```python
# RenderingEngineTypeType definition

RenderingEngineTypeType = Literal[
    "OGRE",
]
```
## RobotDeploymentStepType

```python
# RobotDeploymentStepType usage example

from types_aiobotocore_robomaker.literals import RobotDeploymentStepType

def get_value() -> RobotDeploymentStepType:
    return "DownloadingExtracting"
```

```python
# RobotDeploymentStepType definition

RobotDeploymentStepType = Literal[
    "DownloadingExtracting",
    "ExecutingDownloadCondition",
    "ExecutingPostLaunch",
    "ExecutingPreLaunch",
    "Finished",
    "Launching",
    "Validating",
]
```
## RobotSoftwareSuiteTypeType

```python
# RobotSoftwareSuiteTypeType usage example

from types_aiobotocore_robomaker.literals import RobotSoftwareSuiteTypeType

def get_value() -> RobotSoftwareSuiteTypeType:
    return "General"
```

```python
# RobotSoftwareSuiteTypeType definition

RobotSoftwareSuiteTypeType = Literal[
    "General",
    "ROS",
    "ROS2",
]
```
## RobotSoftwareSuiteVersionTypeType

```python
# RobotSoftwareSuiteVersionTypeType usage example

from types_aiobotocore_robomaker.literals import RobotSoftwareSuiteVersionTypeType

def get_value() -> RobotSoftwareSuiteVersionTypeType:
    return "Dashing"
```

```python
# RobotSoftwareSuiteVersionTypeType definition

RobotSoftwareSuiteVersionTypeType = Literal[
    "Dashing",
    "Foxy",
    "Kinetic",
    "Melodic",
]
```
## RobotStatusType

```python
# RobotStatusType usage example

from types_aiobotocore_robomaker.literals import RobotStatusType

def get_value() -> RobotStatusType:
    return "Available"
```

```python
# RobotStatusType definition

RobotStatusType = Literal[
    "Available",
    "Deploying",
    "Failed",
    "InSync",
    "NoResponse",
    "PendingNewDeployment",
    "Registered",
]
```
## SimulationJobBatchErrorCodeType

```python
# SimulationJobBatchErrorCodeType usage example

from types_aiobotocore_robomaker.literals import SimulationJobBatchErrorCodeType

def get_value() -> SimulationJobBatchErrorCodeType:
    return "InternalServiceError"
```

```python
# SimulationJobBatchErrorCodeType definition

SimulationJobBatchErrorCodeType = Literal[
    "InternalServiceError",
]
```
## SimulationJobBatchStatusType

```python
# SimulationJobBatchStatusType usage example

from types_aiobotocore_robomaker.literals import SimulationJobBatchStatusType

def get_value() -> SimulationJobBatchStatusType:
    return "Canceled"
```

```python
# SimulationJobBatchStatusType definition

SimulationJobBatchStatusType = Literal[
    "Canceled",
    "Canceling",
    "Completed",
    "Completing",
    "Failed",
    "InProgress",
    "Pending",
    "TimedOut",
    "TimingOut",
]
```
## SimulationJobErrorCodeType

```python
# SimulationJobErrorCodeType usage example

from types_aiobotocore_robomaker.literals import SimulationJobErrorCodeType

def get_value() -> SimulationJobErrorCodeType:
    return "BadPermissionsCloudwatchLogs"
```

```python
# SimulationJobErrorCodeType definition

SimulationJobErrorCodeType = Literal[
    "BadPermissionsCloudwatchLogs",
    "BadPermissionsRobotApplication",
    "BadPermissionsS3Object",
    "BadPermissionsS3Output",
    "BadPermissionsSimulationApplication",
    "BadPermissionsUserCredentials",
    "BatchCanceled",
    "BatchTimedOut",
    "ENILimitExceeded",
    "InternalServiceError",
    "InvalidBundleRobotApplication",
    "InvalidBundleSimulationApplication",
    "InvalidInput",
    "InvalidS3Resource",
    "LimitExceeded",
    "MismatchedEtag",
    "RequestThrottled",
    "ResourceNotFound",
    "RobotApplicationCrash",
    "RobotApplicationHealthCheckFailure",
    "RobotApplicationVersionMismatchedEtag",
    "SimulationApplicationCrash",
    "SimulationApplicationHealthCheckFailure",
    "SimulationApplicationVersionMismatchedEtag",
    "SubnetIpLimitExceeded",
    "ThrottlingError",
    "UploadContentMismatchError",
    "WrongRegionRobotApplication",
    "WrongRegionS3Bucket",
    "WrongRegionS3Output",
    "WrongRegionSimulationApplication",
]
```
## SimulationJobStatusType

```python
# SimulationJobStatusType usage example

from types_aiobotocore_robomaker.literals import SimulationJobStatusType

def get_value() -> SimulationJobStatusType:
    return "Canceled"
```

```python
# SimulationJobStatusType definition

SimulationJobStatusType = Literal[
    "Canceled",
    "Completed",
    "Failed",
    "Pending",
    "Preparing",
    "Restarting",
    "Running",
    "RunningFailed",
    "Terminated",
    "Terminating",
]
```
## SimulationSoftwareSuiteTypeType

```python
# SimulationSoftwareSuiteTypeType usage example

from types_aiobotocore_robomaker.literals import SimulationSoftwareSuiteTypeType

def get_value() -> SimulationSoftwareSuiteTypeType:
    return "Gazebo"
```

```python
# SimulationSoftwareSuiteTypeType definition

SimulationSoftwareSuiteTypeType = Literal[
    "Gazebo",
    "RosbagPlay",
    "SimulationRuntime",
]
```
## UploadBehaviorType

```python
# UploadBehaviorType usage example

from types_aiobotocore_robomaker.literals import UploadBehaviorType

def get_value() -> UploadBehaviorType:
    return "UPLOAD_ON_TERMINATE"
```

```python
# UploadBehaviorType definition

UploadBehaviorType = Literal[
    "UPLOAD_ON_TERMINATE",
    "UPLOAD_ROLLING_AUTO_REMOVE",
]
```
## WorldExportJobErrorCodeType

```python
# WorldExportJobErrorCodeType usage example

from types_aiobotocore_robomaker.literals import WorldExportJobErrorCodeType

def get_value() -> WorldExportJobErrorCodeType:
    return "AccessDenied"
```

```python
# WorldExportJobErrorCodeType definition

WorldExportJobErrorCodeType = Literal[
    "AccessDenied",
    "InternalServiceError",
    "InvalidInput",
    "LimitExceeded",
    "RequestThrottled",
    "ResourceNotFound",
]
```
## WorldExportJobStatusType

```python
# WorldExportJobStatusType usage example

from types_aiobotocore_robomaker.literals import WorldExportJobStatusType

def get_value() -> WorldExportJobStatusType:
    return "Canceled"
```

```python
# WorldExportJobStatusType definition

WorldExportJobStatusType = Literal[
    "Canceled",
    "Canceling",
    "Completed",
    "Failed",
    "Pending",
    "Running",
]
```
## WorldGenerationJobErrorCodeType

```python
# WorldGenerationJobErrorCodeType usage example

from types_aiobotocore_robomaker.literals import WorldGenerationJobErrorCodeType

def get_value() -> WorldGenerationJobErrorCodeType:
    return "AllWorldGenerationFailed"
```

```python
# WorldGenerationJobErrorCodeType definition

WorldGenerationJobErrorCodeType = Literal[
    "AllWorldGenerationFailed",
    "InternalServiceError",
    "InvalidInput",
    "LimitExceeded",
    "RequestThrottled",
    "ResourceNotFound",
]
```
## WorldGenerationJobStatusType

```python
# WorldGenerationJobStatusType usage example

from types_aiobotocore_robomaker.literals import WorldGenerationJobStatusType

def get_value() -> WorldGenerationJobStatusType:
    return "Canceled"
```

```python
# WorldGenerationJobStatusType definition

WorldGenerationJobStatusType = Literal[
    "Canceled",
    "Canceling",
    "Completed",
    "Failed",
    "PartialFailed",
    "Pending",
    "Running",
]
```
## RoboMakerServiceName

```python
# RoboMakerServiceName usage example

from types_aiobotocore_robomaker.literals import RoboMakerServiceName

def get_value() -> RoboMakerServiceName:
    return "robomaker"
```

```python
# RoboMakerServiceName definition

RoboMakerServiceName = Literal[
    "robomaker",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_robomaker.literals import ServiceName

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

from types_aiobotocore_robomaker.literals import ResourceServiceName

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

from types_aiobotocore_robomaker.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_deployment_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_deployment_jobs",
    "list_fleets",
    "list_robot_applications",
    "list_robots",
    "list_simulation_applications",
    "list_simulation_job_batches",
    "list_simulation_jobs",
    "list_world_export_jobs",
    "list_world_generation_jobs",
    "list_world_templates",
    "list_worlds",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_robomaker.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "eu-central-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
