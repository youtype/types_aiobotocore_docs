# Literals

> [Index](../README.md) > [Batch](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

## ArrayJobDependencyType

```python
# ArrayJobDependencyType usage example
from types_aiobotocore_batch.literals import ArrayJobDependencyType

def get_value() -> ArrayJobDependencyType:
    return "N_TO_N"
```

```python
# ArrayJobDependencyType definition
ArrayJobDependencyType = Literal[
    "N_TO_N",
    "SEQUENTIAL",
]
```
## AssignPublicIpType

```python
# AssignPublicIpType usage example
from types_aiobotocore_batch.literals import AssignPublicIpType

def get_value() -> AssignPublicIpType:
    return "DISABLED"
```

```python
# AssignPublicIpType definition
AssignPublicIpType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## CEStateType

```python
# CEStateType usage example
from types_aiobotocore_batch.literals import CEStateType

def get_value() -> CEStateType:
    return "DISABLED"
```

```python
# CEStateType definition
CEStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## CEStatusType

```python
# CEStatusType usage example
from types_aiobotocore_batch.literals import CEStatusType

def get_value() -> CEStatusType:
    return "CREATING"
```

```python
# CEStatusType definition
CEStatusType = Literal[
    "CREATING",
    "DELETED",
    "DELETING",
    "INVALID",
    "UPDATING",
    "VALID",
]
```
## CETypeType

```python
# CETypeType usage example
from types_aiobotocore_batch.literals import CETypeType

def get_value() -> CETypeType:
    return "MANAGED"
```

```python
# CETypeType definition
CETypeType = Literal[
    "MANAGED",
    "UNMANAGED",
]
```
## CRAllocationStrategyType

```python
# CRAllocationStrategyType usage example
from types_aiobotocore_batch.literals import CRAllocationStrategyType

def get_value() -> CRAllocationStrategyType:
    return "BEST_FIT"
```

```python
# CRAllocationStrategyType definition
CRAllocationStrategyType = Literal[
    "BEST_FIT",
    "BEST_FIT_PROGRESSIVE",
    "SPOT_CAPACITY_OPTIMIZED",
    "SPOT_PRICE_CAPACITY_OPTIMIZED",
]
```
## CRTypeType

```python
# CRTypeType usage example
from types_aiobotocore_batch.literals import CRTypeType

def get_value() -> CRTypeType:
    return "EC2"
```

```python
# CRTypeType definition
CRTypeType = Literal[
    "EC2",
    "FARGATE",
    "FARGATE_SPOT",
    "SPOT",
]
```
## CRUpdateAllocationStrategyType

```python
# CRUpdateAllocationStrategyType usage example
from types_aiobotocore_batch.literals import CRUpdateAllocationStrategyType

def get_value() -> CRUpdateAllocationStrategyType:
    return "BEST_FIT_PROGRESSIVE"
```

```python
# CRUpdateAllocationStrategyType definition
CRUpdateAllocationStrategyType = Literal[
    "BEST_FIT_PROGRESSIVE",
    "SPOT_CAPACITY_OPTIMIZED",
    "SPOT_PRICE_CAPACITY_OPTIMIZED",
]
```
## DescribeComputeEnvironmentsPaginatorName

```python
# DescribeComputeEnvironmentsPaginatorName usage example
from types_aiobotocore_batch.literals import DescribeComputeEnvironmentsPaginatorName

def get_value() -> DescribeComputeEnvironmentsPaginatorName:
    return "describe_compute_environments"
```

```python
# DescribeComputeEnvironmentsPaginatorName definition
DescribeComputeEnvironmentsPaginatorName = Literal[
    "describe_compute_environments",
]
```
## DescribeJobDefinitionsPaginatorName

```python
# DescribeJobDefinitionsPaginatorName usage example
from types_aiobotocore_batch.literals import DescribeJobDefinitionsPaginatorName

def get_value() -> DescribeJobDefinitionsPaginatorName:
    return "describe_job_definitions"
```

```python
# DescribeJobDefinitionsPaginatorName definition
DescribeJobDefinitionsPaginatorName = Literal[
    "describe_job_definitions",
]
```
## DescribeJobQueuesPaginatorName

```python
# DescribeJobQueuesPaginatorName usage example
from types_aiobotocore_batch.literals import DescribeJobQueuesPaginatorName

def get_value() -> DescribeJobQueuesPaginatorName:
    return "describe_job_queues"
```

```python
# DescribeJobQueuesPaginatorName definition
DescribeJobQueuesPaginatorName = Literal[
    "describe_job_queues",
]
```
## DeviceCgroupPermissionType

```python
# DeviceCgroupPermissionType usage example
from types_aiobotocore_batch.literals import DeviceCgroupPermissionType

def get_value() -> DeviceCgroupPermissionType:
    return "MKNOD"
```

```python
# DeviceCgroupPermissionType definition
DeviceCgroupPermissionType = Literal[
    "MKNOD",
    "READ",
    "WRITE",
]
```
## EFSAuthorizationConfigIAMType

```python
# EFSAuthorizationConfigIAMType usage example
from types_aiobotocore_batch.literals import EFSAuthorizationConfigIAMType

def get_value() -> EFSAuthorizationConfigIAMType:
    return "DISABLED"
```

```python
# EFSAuthorizationConfigIAMType definition
EFSAuthorizationConfigIAMType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EFSTransitEncryptionType

```python
# EFSTransitEncryptionType usage example
from types_aiobotocore_batch.literals import EFSTransitEncryptionType

def get_value() -> EFSTransitEncryptionType:
    return "DISABLED"
```

```python
# EFSTransitEncryptionType definition
EFSTransitEncryptionType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## JQStateType

```python
# JQStateType usage example
from types_aiobotocore_batch.literals import JQStateType

def get_value() -> JQStateType:
    return "DISABLED"
```

```python
# JQStateType definition
JQStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## JQStatusType

```python
# JQStatusType usage example
from types_aiobotocore_batch.literals import JQStatusType

def get_value() -> JQStatusType:
    return "CREATING"
```

```python
# JQStatusType definition
JQStatusType = Literal[
    "CREATING",
    "DELETED",
    "DELETING",
    "INVALID",
    "UPDATING",
    "VALID",
]
```
## JobDefinitionTypeType

```python
# JobDefinitionTypeType usage example
from types_aiobotocore_batch.literals import JobDefinitionTypeType

def get_value() -> JobDefinitionTypeType:
    return "container"
```

```python
# JobDefinitionTypeType definition
JobDefinitionTypeType = Literal[
    "container",
    "multinode",
]
```
## JobStateTimeLimitActionsActionType

```python
# JobStateTimeLimitActionsActionType usage example
from types_aiobotocore_batch.literals import JobStateTimeLimitActionsActionType

def get_value() -> JobStateTimeLimitActionsActionType:
    return "CANCEL"
```

```python
# JobStateTimeLimitActionsActionType definition
JobStateTimeLimitActionsActionType = Literal[
    "CANCEL",
]
```
## JobStateTimeLimitActionsStateType

```python
# JobStateTimeLimitActionsStateType usage example
from types_aiobotocore_batch.literals import JobStateTimeLimitActionsStateType

def get_value() -> JobStateTimeLimitActionsStateType:
    return "RUNNABLE"
```

```python
# JobStateTimeLimitActionsStateType definition
JobStateTimeLimitActionsStateType = Literal[
    "RUNNABLE",
]
```
## JobStatusType

```python
# JobStatusType usage example
from types_aiobotocore_batch.literals import JobStatusType

def get_value() -> JobStatusType:
    return "FAILED"
```

```python
# JobStatusType definition
JobStatusType = Literal[
    "FAILED",
    "PENDING",
    "RUNNABLE",
    "RUNNING",
    "STARTING",
    "SUBMITTED",
    "SUCCEEDED",
]
```
## ListJobsPaginatorName

```python
# ListJobsPaginatorName usage example
from types_aiobotocore_batch.literals import ListJobsPaginatorName

def get_value() -> ListJobsPaginatorName:
    return "list_jobs"
```

```python
# ListJobsPaginatorName definition
ListJobsPaginatorName = Literal[
    "list_jobs",
]
```
## ListSchedulingPoliciesPaginatorName

```python
# ListSchedulingPoliciesPaginatorName usage example
from types_aiobotocore_batch.literals import ListSchedulingPoliciesPaginatorName

def get_value() -> ListSchedulingPoliciesPaginatorName:
    return "list_scheduling_policies"
```

```python
# ListSchedulingPoliciesPaginatorName definition
ListSchedulingPoliciesPaginatorName = Literal[
    "list_scheduling_policies",
]
```
## LogDriverType

```python
# LogDriverType usage example
from types_aiobotocore_batch.literals import LogDriverType

def get_value() -> LogDriverType:
    return "awslogs"
```

```python
# LogDriverType definition
LogDriverType = Literal[
    "awslogs",
    "fluentd",
    "gelf",
    "journald",
    "json-file",
    "splunk",
    "syslog",
]
```
## OrchestrationTypeType

```python
# OrchestrationTypeType usage example
from types_aiobotocore_batch.literals import OrchestrationTypeType

def get_value() -> OrchestrationTypeType:
    return "ECS"
```

```python
# OrchestrationTypeType definition
OrchestrationTypeType = Literal[
    "ECS",
    "EKS",
]
```
## PlatformCapabilityType

```python
# PlatformCapabilityType usage example
from types_aiobotocore_batch.literals import PlatformCapabilityType

def get_value() -> PlatformCapabilityType:
    return "EC2"
```

```python
# PlatformCapabilityType definition
PlatformCapabilityType = Literal[
    "EC2",
    "FARGATE",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example
from types_aiobotocore_batch.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "GPU"
```

```python
# ResourceTypeType definition
ResourceTypeType = Literal[
    "GPU",
    "MEMORY",
    "VCPU",
]
```
## RetryActionType

```python
# RetryActionType usage example
from types_aiobotocore_batch.literals import RetryActionType

def get_value() -> RetryActionType:
    return "EXIT"
```

```python
# RetryActionType definition
RetryActionType = Literal[
    "EXIT",
    "RETRY",
]
```
## BatchServiceName

```python
# BatchServiceName usage example
from types_aiobotocore_batch.literals import BatchServiceName

def get_value() -> BatchServiceName:
    return "batch"
```

```python
# BatchServiceName definition
BatchServiceName = Literal[
    "batch",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_batch.literals import ServiceName

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
from types_aiobotocore_batch.literals import ResourceServiceName

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
from types_aiobotocore_batch.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_compute_environments"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_compute_environments",
    "describe_job_definitions",
    "describe_job_queues",
    "list_jobs",
    "list_scheduling_policies",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_batch.literals import RegionName

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
    "ca-west-1",
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
    "mx-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
