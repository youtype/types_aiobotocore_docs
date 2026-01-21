# Literals

> [Index](../README.md) > [ParallelComputingService](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## AccountingModeType

```python
# AccountingModeType usage example
from types_aiobotocore_pcs.literals import AccountingModeType

def get_value() -> AccountingModeType:
    return "NONE"
```

```python
# AccountingModeType definition
AccountingModeType = Literal[
    "NONE",
    "STANDARD",
]
```
## ClusterStatusType

```python
# ClusterStatusType usage example
from types_aiobotocore_pcs.literals import ClusterStatusType

def get_value() -> ClusterStatusType:
    return "ACTIVE"
```

```python
# ClusterStatusType definition
ClusterStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
    "SUSPENDED",
    "SUSPENDING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ComputeNodeGroupStatusType

```python
# ComputeNodeGroupStatusType usage example
from types_aiobotocore_pcs.literals import ComputeNodeGroupStatusType

def get_value() -> ComputeNodeGroupStatusType:
    return "ACTIVE"
```

```python
# ComputeNodeGroupStatusType definition
ComputeNodeGroupStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "SUSPENDED",
    "SUSPENDING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## EndpointTypeType

```python
# EndpointTypeType usage example
from types_aiobotocore_pcs.literals import EndpointTypeType

def get_value() -> EndpointTypeType:
    return "SLURMCTLD"
```

```python
# EndpointTypeType definition
EndpointTypeType = Literal[
    "SLURMCTLD",
    "SLURMDBD",
    "SLURMRESTD",
]
```
## ListClustersPaginatorName

```python
# ListClustersPaginatorName usage example
from types_aiobotocore_pcs.literals import ListClustersPaginatorName

def get_value() -> ListClustersPaginatorName:
    return "list_clusters"
```

```python
# ListClustersPaginatorName definition
ListClustersPaginatorName = Literal[
    "list_clusters",
]
```
## ListComputeNodeGroupsPaginatorName

```python
# ListComputeNodeGroupsPaginatorName usage example
from types_aiobotocore_pcs.literals import ListComputeNodeGroupsPaginatorName

def get_value() -> ListComputeNodeGroupsPaginatorName:
    return "list_compute_node_groups"
```

```python
# ListComputeNodeGroupsPaginatorName definition
ListComputeNodeGroupsPaginatorName = Literal[
    "list_compute_node_groups",
]
```
## ListQueuesPaginatorName

```python
# ListQueuesPaginatorName usage example
from types_aiobotocore_pcs.literals import ListQueuesPaginatorName

def get_value() -> ListQueuesPaginatorName:
    return "list_queues"
```

```python
# ListQueuesPaginatorName definition
ListQueuesPaginatorName = Literal[
    "list_queues",
]
```
## NetworkTypeType

```python
# NetworkTypeType usage example
from types_aiobotocore_pcs.literals import NetworkTypeType

def get_value() -> NetworkTypeType:
    return "IPV4"
```

```python
# NetworkTypeType definition
NetworkTypeType = Literal[
    "IPV4",
    "IPV6",
]
```
## PurchaseOptionType

```python
# PurchaseOptionType usage example
from types_aiobotocore_pcs.literals import PurchaseOptionType

def get_value() -> PurchaseOptionType:
    return "CAPACITY_BLOCK"
```

```python
# PurchaseOptionType definition
PurchaseOptionType = Literal[
    "CAPACITY_BLOCK",
    "ONDEMAND",
    "SPOT",
]
```
## QueueStatusType

```python
# QueueStatusType usage example
from types_aiobotocore_pcs.literals import QueueStatusType

def get_value() -> QueueStatusType:
    return "ACTIVE"
```

```python
# QueueStatusType definition
QueueStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
    "SUSPENDED",
    "SUSPENDING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## SchedulerTypeType

```python
# SchedulerTypeType usage example
from types_aiobotocore_pcs.literals import SchedulerTypeType

def get_value() -> SchedulerTypeType:
    return "SLURM"
```

```python
# SchedulerTypeType definition
SchedulerTypeType = Literal[
    "SLURM",
]
```
## SizeType

```python
# SizeType usage example
from types_aiobotocore_pcs.literals import SizeType

def get_value() -> SizeType:
    return "LARGE"
```

```python
# SizeType definition
SizeType = Literal[
    "LARGE",
    "MEDIUM",
    "SMALL",
]
```
## SlurmRestModeType

```python
# SlurmRestModeType usage example
from types_aiobotocore_pcs.literals import SlurmRestModeType

def get_value() -> SlurmRestModeType:
    return "NONE"
```

```python
# SlurmRestModeType definition
SlurmRestModeType = Literal[
    "NONE",
    "STANDARD",
]
```
## SpotAllocationStrategyType

```python
# SpotAllocationStrategyType usage example
from types_aiobotocore_pcs.literals import SpotAllocationStrategyType

def get_value() -> SpotAllocationStrategyType:
    return "capacity-optimized"
```

```python
# SpotAllocationStrategyType definition
SpotAllocationStrategyType = Literal[
    "capacity-optimized",
    "lowest-price",
    "price-capacity-optimized",
]
```
## ParallelComputingServiceServiceName

```python
# ParallelComputingServiceServiceName usage example
from types_aiobotocore_pcs.literals import ParallelComputingServiceServiceName

def get_value() -> ParallelComputingServiceServiceName:
    return "pcs"
```

```python
# ParallelComputingServiceServiceName definition
ParallelComputingServiceServiceName = Literal[
    "pcs",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_pcs.literals import ServiceName

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
from types_aiobotocore_pcs.literals import ResourceServiceName

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
from types_aiobotocore_pcs.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_clusters"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_clusters",
    "list_compute_node_groups",
    "list_queues",
]
```
