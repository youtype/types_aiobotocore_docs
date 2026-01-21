# Literals

> [Index](../README.md) > [Kinesis](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## ConsumerStatusType

```python
# ConsumerStatusType usage example
from types_aiobotocore_kinesis.literals import ConsumerStatusType

def get_value() -> ConsumerStatusType:
    return "ACTIVE"
```

```python
# ConsumerStatusType definition
ConsumerStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
]
```
## DescribeStreamPaginatorName

```python
# DescribeStreamPaginatorName usage example
from types_aiobotocore_kinesis.literals import DescribeStreamPaginatorName

def get_value() -> DescribeStreamPaginatorName:
    return "describe_stream"
```

```python
# DescribeStreamPaginatorName definition
DescribeStreamPaginatorName = Literal[
    "describe_stream",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example
from types_aiobotocore_kinesis.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "KMS"
```

```python
# EncryptionTypeType definition
EncryptionTypeType = Literal[
    "KMS",
    "NONE",
]
```
## ListShardsPaginatorName

```python
# ListShardsPaginatorName usage example
from types_aiobotocore_kinesis.literals import ListShardsPaginatorName

def get_value() -> ListShardsPaginatorName:
    return "list_shards"
```

```python
# ListShardsPaginatorName definition
ListShardsPaginatorName = Literal[
    "list_shards",
]
```
## ListStreamConsumersPaginatorName

```python
# ListStreamConsumersPaginatorName usage example
from types_aiobotocore_kinesis.literals import ListStreamConsumersPaginatorName

def get_value() -> ListStreamConsumersPaginatorName:
    return "list_stream_consumers"
```

```python
# ListStreamConsumersPaginatorName definition
ListStreamConsumersPaginatorName = Literal[
    "list_stream_consumers",
]
```
## ListStreamsPaginatorName

```python
# ListStreamsPaginatorName usage example
from types_aiobotocore_kinesis.literals import ListStreamsPaginatorName

def get_value() -> ListStreamsPaginatorName:
    return "list_streams"
```

```python
# ListStreamsPaginatorName definition
ListStreamsPaginatorName = Literal[
    "list_streams",
]
```
## MetricsNameType

```python
# MetricsNameType usage example
from types_aiobotocore_kinesis.literals import MetricsNameType

def get_value() -> MetricsNameType:
    return "ALL"
```

```python
# MetricsNameType definition
MetricsNameType = Literal[
    "ALL",
    "IncomingBytes",
    "IncomingRecords",
    "IteratorAgeMilliseconds",
    "OutgoingBytes",
    "OutgoingRecords",
    "ReadProvisionedThroughputExceeded",
    "WriteProvisionedThroughputExceeded",
]
```
## MinimumThroughputBillingCommitmentInputStatusType

```python
# MinimumThroughputBillingCommitmentInputStatusType usage example
from types_aiobotocore_kinesis.literals import MinimumThroughputBillingCommitmentInputStatusType

def get_value() -> MinimumThroughputBillingCommitmentInputStatusType:
    return "DISABLED"
```

```python
# MinimumThroughputBillingCommitmentInputStatusType definition
MinimumThroughputBillingCommitmentInputStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## MinimumThroughputBillingCommitmentOutputStatusType

```python
# MinimumThroughputBillingCommitmentOutputStatusType usage example
from types_aiobotocore_kinesis.literals import MinimumThroughputBillingCommitmentOutputStatusType

def get_value() -> MinimumThroughputBillingCommitmentOutputStatusType:
    return "DISABLED"
```

```python
# MinimumThroughputBillingCommitmentOutputStatusType definition
MinimumThroughputBillingCommitmentOutputStatusType = Literal[
    "DISABLED",
    "ENABLED",
    "ENABLED_UNTIL_EARLIEST_ALLOWED_END",
]
```
## ScalingTypeType

```python
# ScalingTypeType usage example
from types_aiobotocore_kinesis.literals import ScalingTypeType

def get_value() -> ScalingTypeType:
    return "UNIFORM_SCALING"
```

```python
# ScalingTypeType definition
ScalingTypeType = Literal[
    "UNIFORM_SCALING",
]
```
## ShardFilterTypeType

```python
# ShardFilterTypeType usage example
from types_aiobotocore_kinesis.literals import ShardFilterTypeType

def get_value() -> ShardFilterTypeType:
    return "AFTER_SHARD_ID"
```

```python
# ShardFilterTypeType definition
ShardFilterTypeType = Literal[
    "AFTER_SHARD_ID",
    "AT_LATEST",
    "AT_TIMESTAMP",
    "AT_TRIM_HORIZON",
    "FROM_TIMESTAMP",
    "FROM_TRIM_HORIZON",
]
```
## ShardIteratorTypeType

```python
# ShardIteratorTypeType usage example
from types_aiobotocore_kinesis.literals import ShardIteratorTypeType

def get_value() -> ShardIteratorTypeType:
    return "AFTER_SEQUENCE_NUMBER"
```

```python
# ShardIteratorTypeType definition
ShardIteratorTypeType = Literal[
    "AFTER_SEQUENCE_NUMBER",
    "AT_SEQUENCE_NUMBER",
    "AT_TIMESTAMP",
    "LATEST",
    "TRIM_HORIZON",
]
```
## StreamExistsWaiterName

```python
# StreamExistsWaiterName usage example
from types_aiobotocore_kinesis.literals import StreamExistsWaiterName

def get_value() -> StreamExistsWaiterName:
    return "stream_exists"
```

```python
# StreamExistsWaiterName definition
StreamExistsWaiterName = Literal[
    "stream_exists",
]
```
## StreamModeType

```python
# StreamModeType usage example
from types_aiobotocore_kinesis.literals import StreamModeType

def get_value() -> StreamModeType:
    return "ON_DEMAND"
```

```python
# StreamModeType definition
StreamModeType = Literal[
    "ON_DEMAND",
    "PROVISIONED",
]
```
## StreamNotExistsWaiterName

```python
# StreamNotExistsWaiterName usage example
from types_aiobotocore_kinesis.literals import StreamNotExistsWaiterName

def get_value() -> StreamNotExistsWaiterName:
    return "stream_not_exists"
```

```python
# StreamNotExistsWaiterName definition
StreamNotExistsWaiterName = Literal[
    "stream_not_exists",
]
```
## StreamStatusType

```python
# StreamStatusType usage example
from types_aiobotocore_kinesis.literals import StreamStatusType

def get_value() -> StreamStatusType:
    return "ACTIVE"
```

```python
# StreamStatusType definition
StreamStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "UPDATING",
]
```
## KinesisServiceName

```python
# KinesisServiceName usage example
from types_aiobotocore_kinesis.literals import KinesisServiceName

def get_value() -> KinesisServiceName:
    return "kinesis"
```

```python
# KinesisServiceName definition
KinesisServiceName = Literal[
    "kinesis",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_kinesis.literals import ServiceName

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
from types_aiobotocore_kinesis.literals import ResourceServiceName

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
from types_aiobotocore_kinesis.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_stream"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_stream",
    "list_shards",
    "list_stream_consumers",
    "list_streams",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_kinesis.literals import WaiterName

def get_value() -> WaiterName:
    return "stream_exists"
```

```python
# WaiterName definition
WaiterName = Literal[
    "stream_exists",
    "stream_not_exists",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_kinesis.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition
RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-east-2",
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
    "ap-southeast-6",
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
