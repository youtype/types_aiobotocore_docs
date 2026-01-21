# Literals

> [Index](../README.md) > [Kafka](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## BrokerAZDistributionType

```python
# BrokerAZDistributionType usage example
from types_aiobotocore_kafka.literals import BrokerAZDistributionType

def get_value() -> BrokerAZDistributionType:
    return "DEFAULT"
```

```python
# BrokerAZDistributionType definition
BrokerAZDistributionType = Literal[
    "DEFAULT",
]
```
## ClientBrokerType

```python
# ClientBrokerType usage example
from types_aiobotocore_kafka.literals import ClientBrokerType

def get_value() -> ClientBrokerType:
    return "PLAINTEXT"
```

```python
# ClientBrokerType definition
ClientBrokerType = Literal[
    "PLAINTEXT",
    "TLS",
    "TLS_PLAINTEXT",
]
```
## ClusterStateType

```python
# ClusterStateType usage example
from types_aiobotocore_kafka.literals import ClusterStateType

def get_value() -> ClusterStateType:
    return "ACTIVE"
```

```python
# ClusterStateType definition
ClusterStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "HEALING",
    "MAINTENANCE",
    "REBOOTING_BROKER",
    "UPDATING",
]
```
## ClusterTypeType

```python
# ClusterTypeType usage example
from types_aiobotocore_kafka.literals import ClusterTypeType

def get_value() -> ClusterTypeType:
    return "PROVISIONED"
```

```python
# ClusterTypeType definition
ClusterTypeType = Literal[
    "PROVISIONED",
    "SERVERLESS",
]
```
## ConfigurationStateType

```python
# ConfigurationStateType usage example
from types_aiobotocore_kafka.literals import ConfigurationStateType

def get_value() -> ConfigurationStateType:
    return "ACTIVE"
```

```python
# ConfigurationStateType definition
ConfigurationStateType = Literal[
    "ACTIVE",
    "DELETE_FAILED",
    "DELETING",
]
```
## CustomerActionStatusType

```python
# CustomerActionStatusType usage example
from types_aiobotocore_kafka.literals import CustomerActionStatusType

def get_value() -> CustomerActionStatusType:
    return "ACTION_RECOMMENDED"
```

```python
# CustomerActionStatusType definition
CustomerActionStatusType = Literal[
    "ACTION_RECOMMENDED",
    "CRITICAL_ACTION_REQUIRED",
    "NONE",
]
```
## DescribeTopicPartitionsPaginatorName

```python
# DescribeTopicPartitionsPaginatorName usage example
from types_aiobotocore_kafka.literals import DescribeTopicPartitionsPaginatorName

def get_value() -> DescribeTopicPartitionsPaginatorName:
    return "describe_topic_partitions"
```

```python
# DescribeTopicPartitionsPaginatorName definition
DescribeTopicPartitionsPaginatorName = Literal[
    "describe_topic_partitions",
]
```
## EnhancedMonitoringType

```python
# EnhancedMonitoringType usage example
from types_aiobotocore_kafka.literals import EnhancedMonitoringType

def get_value() -> EnhancedMonitoringType:
    return "DEFAULT"
```

```python
# EnhancedMonitoringType definition
EnhancedMonitoringType = Literal[
    "DEFAULT",
    "PER_BROKER",
    "PER_TOPIC_PER_BROKER",
    "PER_TOPIC_PER_PARTITION",
]
```
## KafkaVersionStatusType

```python
# KafkaVersionStatusType usage example
from types_aiobotocore_kafka.literals import KafkaVersionStatusType

def get_value() -> KafkaVersionStatusType:
    return "ACTIVE"
```

```python
# KafkaVersionStatusType definition
KafkaVersionStatusType = Literal[
    "ACTIVE",
    "DEPRECATED",
]
```
## ListClientVpcConnectionsPaginatorName

```python
# ListClientVpcConnectionsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListClientVpcConnectionsPaginatorName

def get_value() -> ListClientVpcConnectionsPaginatorName:
    return "list_client_vpc_connections"
```

```python
# ListClientVpcConnectionsPaginatorName definition
ListClientVpcConnectionsPaginatorName = Literal[
    "list_client_vpc_connections",
]
```
## ListClusterOperationsPaginatorName

```python
# ListClusterOperationsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListClusterOperationsPaginatorName

def get_value() -> ListClusterOperationsPaginatorName:
    return "list_cluster_operations"
```

```python
# ListClusterOperationsPaginatorName definition
ListClusterOperationsPaginatorName = Literal[
    "list_cluster_operations",
]
```
## ListClusterOperationsV2PaginatorName

```python
# ListClusterOperationsV2PaginatorName usage example
from types_aiobotocore_kafka.literals import ListClusterOperationsV2PaginatorName

def get_value() -> ListClusterOperationsV2PaginatorName:
    return "list_cluster_operations_v2"
```

```python
# ListClusterOperationsV2PaginatorName definition
ListClusterOperationsV2PaginatorName = Literal[
    "list_cluster_operations_v2",
]
```
## ListClustersPaginatorName

```python
# ListClustersPaginatorName usage example
from types_aiobotocore_kafka.literals import ListClustersPaginatorName

def get_value() -> ListClustersPaginatorName:
    return "list_clusters"
```

```python
# ListClustersPaginatorName definition
ListClustersPaginatorName = Literal[
    "list_clusters",
]
```
## ListClustersV2PaginatorName

```python
# ListClustersV2PaginatorName usage example
from types_aiobotocore_kafka.literals import ListClustersV2PaginatorName

def get_value() -> ListClustersV2PaginatorName:
    return "list_clusters_v2"
```

```python
# ListClustersV2PaginatorName definition
ListClustersV2PaginatorName = Literal[
    "list_clusters_v2",
]
```
## ListConfigurationRevisionsPaginatorName

```python
# ListConfigurationRevisionsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListConfigurationRevisionsPaginatorName

def get_value() -> ListConfigurationRevisionsPaginatorName:
    return "list_configuration_revisions"
```

```python
# ListConfigurationRevisionsPaginatorName definition
ListConfigurationRevisionsPaginatorName = Literal[
    "list_configuration_revisions",
]
```
## ListConfigurationsPaginatorName

```python
# ListConfigurationsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListConfigurationsPaginatorName

def get_value() -> ListConfigurationsPaginatorName:
    return "list_configurations"
```

```python
# ListConfigurationsPaginatorName definition
ListConfigurationsPaginatorName = Literal[
    "list_configurations",
]
```
## ListKafkaVersionsPaginatorName

```python
# ListKafkaVersionsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListKafkaVersionsPaginatorName

def get_value() -> ListKafkaVersionsPaginatorName:
    return "list_kafka_versions"
```

```python
# ListKafkaVersionsPaginatorName definition
ListKafkaVersionsPaginatorName = Literal[
    "list_kafka_versions",
]
```
## ListNodesPaginatorName

```python
# ListNodesPaginatorName usage example
from types_aiobotocore_kafka.literals import ListNodesPaginatorName

def get_value() -> ListNodesPaginatorName:
    return "list_nodes"
```

```python
# ListNodesPaginatorName definition
ListNodesPaginatorName = Literal[
    "list_nodes",
]
```
## ListReplicatorsPaginatorName

```python
# ListReplicatorsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListReplicatorsPaginatorName

def get_value() -> ListReplicatorsPaginatorName:
    return "list_replicators"
```

```python
# ListReplicatorsPaginatorName definition
ListReplicatorsPaginatorName = Literal[
    "list_replicators",
]
```
## ListScramSecretsPaginatorName

```python
# ListScramSecretsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListScramSecretsPaginatorName

def get_value() -> ListScramSecretsPaginatorName:
    return "list_scram_secrets"
```

```python
# ListScramSecretsPaginatorName definition
ListScramSecretsPaginatorName = Literal[
    "list_scram_secrets",
]
```
## ListTopicsPaginatorName

```python
# ListTopicsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListTopicsPaginatorName

def get_value() -> ListTopicsPaginatorName:
    return "list_topics"
```

```python
# ListTopicsPaginatorName definition
ListTopicsPaginatorName = Literal[
    "list_topics",
]
```
## ListVpcConnectionsPaginatorName

```python
# ListVpcConnectionsPaginatorName usage example
from types_aiobotocore_kafka.literals import ListVpcConnectionsPaginatorName

def get_value() -> ListVpcConnectionsPaginatorName:
    return "list_vpc_connections"
```

```python
# ListVpcConnectionsPaginatorName definition
ListVpcConnectionsPaginatorName = Literal[
    "list_vpc_connections",
]
```
## NodeTypeType

```python
# NodeTypeType usage example
from types_aiobotocore_kafka.literals import NodeTypeType

def get_value() -> NodeTypeType:
    return "BROKER"
```

```python
# NodeTypeType definition
NodeTypeType = Literal[
    "BROKER",
]
```
## RebalancingStatusType

```python
# RebalancingStatusType usage example
from types_aiobotocore_kafka.literals import RebalancingStatusType

def get_value() -> RebalancingStatusType:
    return "ACTIVE"
```

```python
# RebalancingStatusType definition
RebalancingStatusType = Literal[
    "ACTIVE",
    "PAUSED",
]
```
## ReplicationStartingPositionTypeType

```python
# ReplicationStartingPositionTypeType usage example
from types_aiobotocore_kafka.literals import ReplicationStartingPositionTypeType

def get_value() -> ReplicationStartingPositionTypeType:
    return "EARLIEST"
```

```python
# ReplicationStartingPositionTypeType definition
ReplicationStartingPositionTypeType = Literal[
    "EARLIEST",
    "LATEST",
]
```
## ReplicationTopicNameConfigurationTypeType

```python
# ReplicationTopicNameConfigurationTypeType usage example
from types_aiobotocore_kafka.literals import ReplicationTopicNameConfigurationTypeType

def get_value() -> ReplicationTopicNameConfigurationTypeType:
    return "IDENTICAL"
```

```python
# ReplicationTopicNameConfigurationTypeType definition
ReplicationTopicNameConfigurationTypeType = Literal[
    "IDENTICAL",
    "PREFIXED_WITH_SOURCE_CLUSTER_ALIAS",
]
```
## ReplicatorStateType

```python
# ReplicatorStateType usage example
from types_aiobotocore_kafka.literals import ReplicatorStateType

def get_value() -> ReplicatorStateType:
    return "CREATING"
```

```python
# ReplicatorStateType definition
ReplicatorStateType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "RUNNING",
    "UPDATING",
]
```
## StorageModeType

```python
# StorageModeType usage example
from types_aiobotocore_kafka.literals import StorageModeType

def get_value() -> StorageModeType:
    return "LOCAL"
```

```python
# StorageModeType definition
StorageModeType = Literal[
    "LOCAL",
    "TIERED",
]
```
## TargetCompressionTypeType

```python
# TargetCompressionTypeType usage example
from types_aiobotocore_kafka.literals import TargetCompressionTypeType

def get_value() -> TargetCompressionTypeType:
    return "GZIP"
```

```python
# TargetCompressionTypeType definition
TargetCompressionTypeType = Literal[
    "GZIP",
    "LZ4",
    "NONE",
    "SNAPPY",
    "ZSTD",
]
```
## TopicStateType

```python
# TopicStateType usage example
from types_aiobotocore_kafka.literals import TopicStateType

def get_value() -> TopicStateType:
    return "ACTIVE"
```

```python
# TopicStateType definition
TopicStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "UPDATING",
]
```
## UserIdentityTypeType

```python
# UserIdentityTypeType usage example
from types_aiobotocore_kafka.literals import UserIdentityTypeType

def get_value() -> UserIdentityTypeType:
    return "AWSACCOUNT"
```

```python
# UserIdentityTypeType definition
UserIdentityTypeType = Literal[
    "AWSACCOUNT",
    "AWSSERVICE",
]
```
## VpcConnectionStateType

```python
# VpcConnectionStateType usage example
from types_aiobotocore_kafka.literals import VpcConnectionStateType

def get_value() -> VpcConnectionStateType:
    return "AVAILABLE"
```

```python
# VpcConnectionStateType definition
VpcConnectionStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "DEACTIVATING",
    "DELETING",
    "FAILED",
    "INACTIVE",
    "REJECTED",
    "REJECTING",
]
```
## KafkaServiceName

```python
# KafkaServiceName usage example
from types_aiobotocore_kafka.literals import KafkaServiceName

def get_value() -> KafkaServiceName:
    return "kafka"
```

```python
# KafkaServiceName definition
KafkaServiceName = Literal[
    "kafka",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_kafka.literals import ServiceName

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
from types_aiobotocore_kafka.literals import ResourceServiceName

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
from types_aiobotocore_kafka.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_topic_partitions"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_topic_partitions",
    "list_client_vpc_connections",
    "list_cluster_operations",
    "list_cluster_operations_v2",
    "list_clusters",
    "list_clusters_v2",
    "list_configuration_revisions",
    "list_configurations",
    "list_kafka_versions",
    "list_nodes",
    "list_replicators",
    "list_scram_secrets",
    "list_topics",
    "list_vpc_connections",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_kafka.literals import RegionName

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
