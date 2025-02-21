# Literals

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#timestreaminfluxdb)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## ClusterDeploymentTypeType

```python
# ClusterDeploymentTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import ClusterDeploymentTypeType

def get_value() -> ClusterDeploymentTypeType:
    return "MULTI_NODE_READ_REPLICAS"
```

```python
# ClusterDeploymentTypeType definition
ClusterDeploymentTypeType = Literal[
    "MULTI_NODE_READ_REPLICAS",
]
```
## ClusterStatusType

```python
# ClusterStatusType usage example
from types_aiobotocore_timestream_influxdb.literals import ClusterStatusType

def get_value() -> ClusterStatusType:
    return "AVAILABLE"
```

```python
# ClusterStatusType definition
ClusterStatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETED",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## DbInstanceTypeType

```python
# DbInstanceTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import DbInstanceTypeType

def get_value() -> DbInstanceTypeType:
    return "db.influx.12xlarge"
```

```python
# DbInstanceTypeType definition
DbInstanceTypeType = Literal[
    "db.influx.12xlarge",
    "db.influx.16xlarge",
    "db.influx.2xlarge",
    "db.influx.4xlarge",
    "db.influx.8xlarge",
    "db.influx.large",
    "db.influx.medium",
    "db.influx.xlarge",
]
```
## DbStorageTypeType

```python
# DbStorageTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import DbStorageTypeType

def get_value() -> DbStorageTypeType:
    return "InfluxIOIncludedT1"
```

```python
# DbStorageTypeType definition
DbStorageTypeType = Literal[
    "InfluxIOIncludedT1",
    "InfluxIOIncludedT2",
    "InfluxIOIncludedT3",
]
```
## DeploymentTypeType

```python
# DeploymentTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import DeploymentTypeType

def get_value() -> DeploymentTypeType:
    return "SINGLE_AZ"
```

```python
# DeploymentTypeType definition
DeploymentTypeType = Literal[
    "SINGLE_AZ",
    "WITH_MULTIAZ_STANDBY",
]
```
## DurationTypeType

```python
# DurationTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import DurationTypeType

def get_value() -> DurationTypeType:
    return "hours"
```

```python
# DurationTypeType definition
DurationTypeType = Literal[
    "hours",
    "milliseconds",
    "minutes",
    "seconds",
]
```
## FailoverModeType

```python
# FailoverModeType usage example
from types_aiobotocore_timestream_influxdb.literals import FailoverModeType

def get_value() -> FailoverModeType:
    return "AUTOMATIC"
```

```python
# FailoverModeType definition
FailoverModeType = Literal[
    "AUTOMATIC",
    "NO_FAILOVER",
]
```
## InstanceModeType

```python
# InstanceModeType usage example
from types_aiobotocore_timestream_influxdb.literals import InstanceModeType

def get_value() -> InstanceModeType:
    return "PRIMARY"
```

```python
# InstanceModeType definition
InstanceModeType = Literal[
    "PRIMARY",
    "REPLICA",
    "STANDBY",
]
```
## ListDbClustersPaginatorName

```python
# ListDbClustersPaginatorName usage example
from types_aiobotocore_timestream_influxdb.literals import ListDbClustersPaginatorName

def get_value() -> ListDbClustersPaginatorName:
    return "list_db_clusters"
```

```python
# ListDbClustersPaginatorName definition
ListDbClustersPaginatorName = Literal[
    "list_db_clusters",
]
```
## ListDbInstancesForClusterPaginatorName

```python
# ListDbInstancesForClusterPaginatorName usage example
from types_aiobotocore_timestream_influxdb.literals import ListDbInstancesForClusterPaginatorName

def get_value() -> ListDbInstancesForClusterPaginatorName:
    return "list_db_instances_for_cluster"
```

```python
# ListDbInstancesForClusterPaginatorName definition
ListDbInstancesForClusterPaginatorName = Literal[
    "list_db_instances_for_cluster",
]
```
## ListDbInstancesPaginatorName

```python
# ListDbInstancesPaginatorName usage example
from types_aiobotocore_timestream_influxdb.literals import ListDbInstancesPaginatorName

def get_value() -> ListDbInstancesPaginatorName:
    return "list_db_instances"
```

```python
# ListDbInstancesPaginatorName definition
ListDbInstancesPaginatorName = Literal[
    "list_db_instances",
]
```
## ListDbParameterGroupsPaginatorName

```python
# ListDbParameterGroupsPaginatorName usage example
from types_aiobotocore_timestream_influxdb.literals import ListDbParameterGroupsPaginatorName

def get_value() -> ListDbParameterGroupsPaginatorName:
    return "list_db_parameter_groups"
```

```python
# ListDbParameterGroupsPaginatorName definition
ListDbParameterGroupsPaginatorName = Literal[
    "list_db_parameter_groups",
]
```
## LogLevelType

```python
# LogLevelType usage example
from types_aiobotocore_timestream_influxdb.literals import LogLevelType

def get_value() -> LogLevelType:
    return "debug"
```

```python
# LogLevelType definition
LogLevelType = Literal[
    "debug",
    "error",
    "info",
]
```
## NetworkTypeType

```python
# NetworkTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import NetworkTypeType

def get_value() -> NetworkTypeType:
    return "DUAL"
```

```python
# NetworkTypeType definition
NetworkTypeType = Literal[
    "DUAL",
    "IPV4",
]
```
## StatusType

```python
# StatusType usage example
from types_aiobotocore_timestream_influxdb.literals import StatusType

def get_value() -> StatusType:
    return "AVAILABLE"
```

```python
# StatusType definition
StatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETED",
    "DELETING",
    "FAILED",
    "MODIFYING",
    "UPDATING",
    "UPDATING_DEPLOYMENT_TYPE",
    "UPDATING_INSTANCE_TYPE",
]
```
## TracingTypeType

```python
# TracingTypeType usage example
from types_aiobotocore_timestream_influxdb.literals import TracingTypeType

def get_value() -> TracingTypeType:
    return "jaeger"
```

```python
# TracingTypeType definition
TracingTypeType = Literal[
    "jaeger",
    "log",
]
```
## TimestreamInfluxDBServiceName

```python
# TimestreamInfluxDBServiceName usage example
from types_aiobotocore_timestream_influxdb.literals import TimestreamInfluxDBServiceName

def get_value() -> TimestreamInfluxDBServiceName:
    return "timestream-influxdb"
```

```python
# TimestreamInfluxDBServiceName definition
TimestreamInfluxDBServiceName = Literal[
    "timestream-influxdb",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_timestream_influxdb.literals import ServiceName

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
from types_aiobotocore_timestream_influxdb.literals import ResourceServiceName

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
from types_aiobotocore_timestream_influxdb.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_db_clusters"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_db_clusters",
    "list_db_instances",
    "list_db_instances_for_cluster",
    "list_db_parameter_groups",
]
```
