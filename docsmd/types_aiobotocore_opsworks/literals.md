# Literals

> [Index](../README.md) > [OpsWorks](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## AppAttributesKeysType

```python
# AppAttributesKeysType usage example
from types_aiobotocore_opsworks.literals import AppAttributesKeysType

def get_value() -> AppAttributesKeysType:
    return "AutoBundleOnDeploy"
```

```python
# AppAttributesKeysType definition
AppAttributesKeysType = Literal[
    "AutoBundleOnDeploy",
    "AwsFlowRubySettings",
    "DocumentRoot",
    "RailsEnv",
]
```
## AppExistsWaiterName

```python
# AppExistsWaiterName usage example
from types_aiobotocore_opsworks.literals import AppExistsWaiterName

def get_value() -> AppExistsWaiterName:
    return "app_exists"
```

```python
# AppExistsWaiterName definition
AppExistsWaiterName = Literal[
    "app_exists",
]
```
## AppTypeType

```python
# AppTypeType usage example
from types_aiobotocore_opsworks.literals import AppTypeType

def get_value() -> AppTypeType:
    return "aws-flow-ruby"
```

```python
# AppTypeType definition
AppTypeType = Literal[
    "aws-flow-ruby",
    "java",
    "nodejs",
    "other",
    "php",
    "rails",
    "static",
]
```
## ArchitectureType

```python
# ArchitectureType usage example
from types_aiobotocore_opsworks.literals import ArchitectureType

def get_value() -> ArchitectureType:
    return "i386"
```

```python
# ArchitectureType definition
ArchitectureType = Literal[
    "i386",
    "x86_64",
]
```
## AutoScalingTypeType

```python
# AutoScalingTypeType usage example
from types_aiobotocore_opsworks.literals import AutoScalingTypeType

def get_value() -> AutoScalingTypeType:
    return "load"
```

```python
# AutoScalingTypeType definition
AutoScalingTypeType = Literal[
    "load",
    "timer",
]
```
## CloudWatchLogsEncodingType

```python
# CloudWatchLogsEncodingType usage example
from types_aiobotocore_opsworks.literals import CloudWatchLogsEncodingType

def get_value() -> CloudWatchLogsEncodingType:
    return "ascii"
```

```python
# CloudWatchLogsEncodingType definition
CloudWatchLogsEncodingType = Literal[
    "ascii",
    "big5",
    "big5hkscs",
    "cp037",
    "cp1006",
    "cp1026",
    "cp1140",
    "cp1250",
    "cp1251",
    "cp1252",
    "cp1253",
    "cp1254",
    "cp1255",
    "cp1256",
    "cp1257",
    "cp1258",
    "cp424",
    "cp437",
    "cp500",
    "cp720",
    "cp737",
    "cp775",
    "cp850",
    "cp852",
    "cp855",
    "cp856",
    "cp857",
    "cp858",
    "cp860",
    "cp861",
    "cp862",
    "cp863",
    "cp864",
    "cp865",
    "cp866",
    "cp869",
    "cp874",
    "cp875",
    "cp932",
    "cp949",
    "cp950",
    "euc_jis_2004",
    "euc_jisx0213",
    "euc_jp",
    "euc_kr",
    "gb18030",
    "gb2312",
    "gbk",
    "hz",
    "iso2022_jp",
    "iso2022_jp_1",
    "iso2022_jp_2",
    "iso2022_jp_2004",
    "iso2022_jp_3",
    "iso2022_jp_ext",
    "iso2022_kr",
    "iso8859_10",
    "iso8859_13",
    "iso8859_14",
    "iso8859_15",
    "iso8859_16",
    "iso8859_2",
    "iso8859_3",
    "iso8859_4",
    "iso8859_5",
    "iso8859_6",
    "iso8859_7",
    "iso8859_8",
    "iso8859_9",
    "johab",
    "koi8_r",
    "koi8_u",
    "latin_1",
    "mac_cyrillic",
    "mac_greek",
    "mac_iceland",
    "mac_latin2",
    "mac_roman",
    "mac_turkish",
    "ptcp154",
    "shift_jis",
    "shift_jis_2004",
    "shift_jisx0213",
    "utf_16",
    "utf_16_be",
    "utf_16_le",
    "utf_32",
    "utf_32_be",
    "utf_32_le",
    "utf_7",
    "utf_8",
    "utf_8_sig",
]
```
## CloudWatchLogsInitialPositionType

```python
# CloudWatchLogsInitialPositionType usage example
from types_aiobotocore_opsworks.literals import CloudWatchLogsInitialPositionType

def get_value() -> CloudWatchLogsInitialPositionType:
    return "end_of_file"
```

```python
# CloudWatchLogsInitialPositionType definition
CloudWatchLogsInitialPositionType = Literal[
    "end_of_file",
    "start_of_file",
]
```
## CloudWatchLogsTimeZoneType

```python
# CloudWatchLogsTimeZoneType usage example
from types_aiobotocore_opsworks.literals import CloudWatchLogsTimeZoneType

def get_value() -> CloudWatchLogsTimeZoneType:
    return "LOCAL"
```

```python
# CloudWatchLogsTimeZoneType definition
CloudWatchLogsTimeZoneType = Literal[
    "LOCAL",
    "UTC",
]
```
## DeploymentCommandNameType

```python
# DeploymentCommandNameType usage example
from types_aiobotocore_opsworks.literals import DeploymentCommandNameType

def get_value() -> DeploymentCommandNameType:
    return "configure"
```

```python
# DeploymentCommandNameType definition
DeploymentCommandNameType = Literal[
    "configure",
    "deploy",
    "execute_recipes",
    "install_dependencies",
    "restart",
    "rollback",
    "setup",
    "start",
    "stop",
    "undeploy",
    "update_custom_cookbooks",
    "update_dependencies",
]
```
## DeploymentSuccessfulWaiterName

```python
# DeploymentSuccessfulWaiterName usage example
from types_aiobotocore_opsworks.literals import DeploymentSuccessfulWaiterName

def get_value() -> DeploymentSuccessfulWaiterName:
    return "deployment_successful"
```

```python
# DeploymentSuccessfulWaiterName definition
DeploymentSuccessfulWaiterName = Literal[
    "deployment_successful",
]
```
## DescribeEcsClustersPaginatorName

```python
# DescribeEcsClustersPaginatorName usage example
from types_aiobotocore_opsworks.literals import DescribeEcsClustersPaginatorName

def get_value() -> DescribeEcsClustersPaginatorName:
    return "describe_ecs_clusters"
```

```python
# DescribeEcsClustersPaginatorName definition
DescribeEcsClustersPaginatorName = Literal[
    "describe_ecs_clusters",
]
```
## InstanceOnlineWaiterName

```python
# InstanceOnlineWaiterName usage example
from types_aiobotocore_opsworks.literals import InstanceOnlineWaiterName

def get_value() -> InstanceOnlineWaiterName:
    return "instance_online"
```

```python
# InstanceOnlineWaiterName definition
InstanceOnlineWaiterName = Literal[
    "instance_online",
]
```
## InstanceRegisteredWaiterName

```python
# InstanceRegisteredWaiterName usage example
from types_aiobotocore_opsworks.literals import InstanceRegisteredWaiterName

def get_value() -> InstanceRegisteredWaiterName:
    return "instance_registered"
```

```python
# InstanceRegisteredWaiterName definition
InstanceRegisteredWaiterName = Literal[
    "instance_registered",
]
```
## InstanceStoppedWaiterName

```python
# InstanceStoppedWaiterName usage example
from types_aiobotocore_opsworks.literals import InstanceStoppedWaiterName

def get_value() -> InstanceStoppedWaiterName:
    return "instance_stopped"
```

```python
# InstanceStoppedWaiterName definition
InstanceStoppedWaiterName = Literal[
    "instance_stopped",
]
```
## InstanceTerminatedWaiterName

```python
# InstanceTerminatedWaiterName usage example
from types_aiobotocore_opsworks.literals import InstanceTerminatedWaiterName

def get_value() -> InstanceTerminatedWaiterName:
    return "instance_terminated"
```

```python
# InstanceTerminatedWaiterName definition
InstanceTerminatedWaiterName = Literal[
    "instance_terminated",
]
```
## LayerAttributesKeysType

```python
# LayerAttributesKeysType usage example
from types_aiobotocore_opsworks.literals import LayerAttributesKeysType

def get_value() -> LayerAttributesKeysType:
    return "BundlerVersion"
```

```python
# LayerAttributesKeysType definition
LayerAttributesKeysType = Literal[
    "BundlerVersion",
    "EcsClusterArn",
    "EnableHaproxyStats",
    "GangliaPassword",
    "GangliaUrl",
    "GangliaUser",
    "HaproxyHealthCheckMethod",
    "HaproxyHealthCheckUrl",
    "HaproxyStatsPassword",
    "HaproxyStatsUrl",
    "HaproxyStatsUser",
    "JavaAppServer",
    "JavaAppServerVersion",
    "Jvm",
    "JvmOptions",
    "JvmVersion",
    "ManageBundler",
    "MemcachedMemory",
    "MysqlRootPassword",
    "MysqlRootPasswordUbiquitous",
    "NodejsVersion",
    "PassengerVersion",
    "RailsStack",
    "RubygemsVersion",
    "RubyVersion",
]
```
## LayerTypeType

```python
# LayerTypeType usage example
from types_aiobotocore_opsworks.literals import LayerTypeType

def get_value() -> LayerTypeType:
    return "aws-flow-ruby"
```

```python
# LayerTypeType definition
LayerTypeType = Literal[
    "aws-flow-ruby",
    "custom",
    "db-master",
    "ecs-cluster",
    "java-app",
    "lb",
    "memcached",
    "monitoring-master",
    "nodejs-app",
    "php-app",
    "rails-app",
    "web",
]
```
## RootDeviceTypeType

```python
# RootDeviceTypeType usage example
from types_aiobotocore_opsworks.literals import RootDeviceTypeType

def get_value() -> RootDeviceTypeType:
    return "ebs"
```

```python
# RootDeviceTypeType definition
RootDeviceTypeType = Literal[
    "ebs",
    "instance-store",
]
```
## SourceTypeType

```python
# SourceTypeType usage example
from types_aiobotocore_opsworks.literals import SourceTypeType

def get_value() -> SourceTypeType:
    return "archive"
```

```python
# SourceTypeType definition
SourceTypeType = Literal[
    "archive",
    "git",
    "s3",
    "svn",
]
```
## StackAttributesKeysType

```python
# StackAttributesKeysType usage example
from types_aiobotocore_opsworks.literals import StackAttributesKeysType

def get_value() -> StackAttributesKeysType:
    return "Color"
```

```python
# StackAttributesKeysType definition
StackAttributesKeysType = Literal[
    "Color",
]
```
## VirtualizationTypeType

```python
# VirtualizationTypeType usage example
from types_aiobotocore_opsworks.literals import VirtualizationTypeType

def get_value() -> VirtualizationTypeType:
    return "hvm"
```

```python
# VirtualizationTypeType definition
VirtualizationTypeType = Literal[
    "hvm",
    "paravirtual",
]
```
## VolumeTypeType

```python
# VolumeTypeType usage example
from types_aiobotocore_opsworks.literals import VolumeTypeType

def get_value() -> VolumeTypeType:
    return "gp2"
```

```python
# VolumeTypeType definition
VolumeTypeType = Literal[
    "gp2",
    "io1",
    "standard",
]
```
## OpsWorksServiceName

```python
# OpsWorksServiceName usage example
from types_aiobotocore_opsworks.literals import OpsWorksServiceName

def get_value() -> OpsWorksServiceName:
    return "opsworks"
```

```python
# OpsWorksServiceName definition
OpsWorksServiceName = Literal[
    "opsworks",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_opsworks.literals import ServiceName

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
from types_aiobotocore_opsworks.literals import ResourceServiceName

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
from types_aiobotocore_opsworks.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_ecs_clusters"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_ecs_clusters",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_opsworks.literals import WaiterName

def get_value() -> WaiterName:
    return "app_exists"
```

```python
# WaiterName definition
WaiterName = Literal[
    "app_exists",
    "deployment_successful",
    "instance_online",
    "instance_registered",
    "instance_stopped",
    "instance_terminated",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_opsworks.literals import RegionName

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
