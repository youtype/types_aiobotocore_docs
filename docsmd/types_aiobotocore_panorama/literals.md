# Literals

> [Index](../README.md) > [Panorama](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## ApplicationInstanceHealthStatusType

```python
# ApplicationInstanceHealthStatusType usage example
from types_aiobotocore_panorama.literals import ApplicationInstanceHealthStatusType

def get_value() -> ApplicationInstanceHealthStatusType:
    return "ERROR"
```

```python
# ApplicationInstanceHealthStatusType definition
ApplicationInstanceHealthStatusType = Literal[
    "ERROR",
    "NOT_AVAILABLE",
    "RUNNING",
]
```
## ApplicationInstanceStatusType

```python
# ApplicationInstanceStatusType usage example
from types_aiobotocore_panorama.literals import ApplicationInstanceStatusType

def get_value() -> ApplicationInstanceStatusType:
    return "DEPLOYMENT_ERROR"
```

```python
# ApplicationInstanceStatusType definition
ApplicationInstanceStatusType = Literal[
    "DEPLOYMENT_ERROR",
    "DEPLOYMENT_FAILED",
    "DEPLOYMENT_IN_PROGRESS",
    "DEPLOYMENT_PENDING",
    "DEPLOYMENT_REQUESTED",
    "DEPLOYMENT_SUCCEEDED",
    "REMOVAL_FAILED",
    "REMOVAL_IN_PROGRESS",
    "REMOVAL_PENDING",
    "REMOVAL_REQUESTED",
    "REMOVAL_SUCCEEDED",
]
```
## ConnectionTypeType

```python
# ConnectionTypeType usage example
from types_aiobotocore_panorama.literals import ConnectionTypeType

def get_value() -> ConnectionTypeType:
    return "DHCP"
```

```python
# ConnectionTypeType definition
ConnectionTypeType = Literal[
    "DHCP",
    "STATIC_IP",
]
```
## DesiredStateType

```python
# DesiredStateType usage example
from types_aiobotocore_panorama.literals import DesiredStateType

def get_value() -> DesiredStateType:
    return "REMOVED"
```

```python
# DesiredStateType definition
DesiredStateType = Literal[
    "REMOVED",
    "RUNNING",
    "STOPPED",
]
```
## DeviceAggregatedStatusType

```python
# DeviceAggregatedStatusType usage example
from types_aiobotocore_panorama.literals import DeviceAggregatedStatusType

def get_value() -> DeviceAggregatedStatusType:
    return "AWAITING_PROVISIONING"
```

```python
# DeviceAggregatedStatusType definition
DeviceAggregatedStatusType = Literal[
    "AWAITING_PROVISIONING",
    "DELETING",
    "ERROR",
    "FAILED",
    "LEASE_EXPIRED",
    "OFFLINE",
    "ONLINE",
    "PENDING",
    "REBOOTING",
    "UPDATE_NEEDED",
]
```
## DeviceBrandType

```python
# DeviceBrandType usage example
from types_aiobotocore_panorama.literals import DeviceBrandType

def get_value() -> DeviceBrandType:
    return "AWS_PANORAMA"
```

```python
# DeviceBrandType definition
DeviceBrandType = Literal[
    "AWS_PANORAMA",
    "LENOVO",
]
```
## DeviceConnectionStatusType

```python
# DeviceConnectionStatusType usage example
from types_aiobotocore_panorama.literals import DeviceConnectionStatusType

def get_value() -> DeviceConnectionStatusType:
    return "AWAITING_CREDENTIALS"
```

```python
# DeviceConnectionStatusType definition
DeviceConnectionStatusType = Literal[
    "AWAITING_CREDENTIALS",
    "ERROR",
    "NOT_AVAILABLE",
    "OFFLINE",
    "ONLINE",
]
```
## DeviceReportedStatusType

```python
# DeviceReportedStatusType usage example
from types_aiobotocore_panorama.literals import DeviceReportedStatusType

def get_value() -> DeviceReportedStatusType:
    return "INSTALL_ERROR"
```

```python
# DeviceReportedStatusType definition
DeviceReportedStatusType = Literal[
    "INSTALL_ERROR",
    "INSTALL_IN_PROGRESS",
    "LAUNCH_ERROR",
    "LAUNCHED",
    "REMOVAL_FAILED",
    "REMOVAL_IN_PROGRESS",
    "RUNNING",
    "STARTING",
    "STOP_ERROR",
    "STOPPED",
    "STOPPING",
]
```
## DeviceStatusType

```python
# DeviceStatusType usage example
from types_aiobotocore_panorama.literals import DeviceStatusType

def get_value() -> DeviceStatusType:
    return "AWAITING_PROVISIONING"
```

```python
# DeviceStatusType definition
DeviceStatusType = Literal[
    "AWAITING_PROVISIONING",
    "DELETING",
    "ERROR",
    "FAILED",
    "PENDING",
    "SUCCEEDED",
]
```
## DeviceTypeType

```python
# DeviceTypeType usage example
from types_aiobotocore_panorama.literals import DeviceTypeType

def get_value() -> DeviceTypeType:
    return "PANORAMA_APPLIANCE"
```

```python
# DeviceTypeType definition
DeviceTypeType = Literal[
    "PANORAMA_APPLIANCE",
    "PANORAMA_APPLIANCE_DEVELOPER_KIT",
]
```
## JobResourceTypeType

```python
# JobResourceTypeType usage example
from types_aiobotocore_panorama.literals import JobResourceTypeType

def get_value() -> JobResourceTypeType:
    return "PACKAGE"
```

```python
# JobResourceTypeType definition
JobResourceTypeType = Literal[
    "PACKAGE",
]
```
## JobTypeType

```python
# JobTypeType usage example
from types_aiobotocore_panorama.literals import JobTypeType

def get_value() -> JobTypeType:
    return "OTA"
```

```python
# JobTypeType definition
JobTypeType = Literal[
    "OTA",
    "REBOOT",
]
```
## ListDevicesSortByType

```python
# ListDevicesSortByType usage example
from types_aiobotocore_panorama.literals import ListDevicesSortByType

def get_value() -> ListDevicesSortByType:
    return "CREATED_TIME"
```

```python
# ListDevicesSortByType definition
ListDevicesSortByType = Literal[
    "CREATED_TIME",
    "DEVICE_AGGREGATED_STATUS",
    "DEVICE_ID",
    "NAME",
]
```
## NetworkConnectionStatusType

```python
# NetworkConnectionStatusType usage example
from types_aiobotocore_panorama.literals import NetworkConnectionStatusType

def get_value() -> NetworkConnectionStatusType:
    return "CONNECTED"
```

```python
# NetworkConnectionStatusType definition
NetworkConnectionStatusType = Literal[
    "CONNECTED",
    "CONNECTING",
    "NOT_CONNECTED",
]
```
## NodeCategoryType

```python
# NodeCategoryType usage example
from types_aiobotocore_panorama.literals import NodeCategoryType

def get_value() -> NodeCategoryType:
    return "BUSINESS_LOGIC"
```

```python
# NodeCategoryType definition
NodeCategoryType = Literal[
    "BUSINESS_LOGIC",
    "MEDIA_SINK",
    "MEDIA_SOURCE",
    "ML_MODEL",
]
```
## NodeFromTemplateJobStatusType

```python
# NodeFromTemplateJobStatusType usage example
from types_aiobotocore_panorama.literals import NodeFromTemplateJobStatusType

def get_value() -> NodeFromTemplateJobStatusType:
    return "FAILED"
```

```python
# NodeFromTemplateJobStatusType definition
NodeFromTemplateJobStatusType = Literal[
    "FAILED",
    "PENDING",
    "SUCCEEDED",
]
```
## NodeInstanceStatusType

```python
# NodeInstanceStatusType usage example
from types_aiobotocore_panorama.literals import NodeInstanceStatusType

def get_value() -> NodeInstanceStatusType:
    return "ERROR"
```

```python
# NodeInstanceStatusType definition
NodeInstanceStatusType = Literal[
    "ERROR",
    "NOT_AVAILABLE",
    "PAUSED",
    "RUNNING",
]
```
## NodeSignalValueType

```python
# NodeSignalValueType usage example
from types_aiobotocore_panorama.literals import NodeSignalValueType

def get_value() -> NodeSignalValueType:
    return "PAUSE"
```

```python
# NodeSignalValueType definition
NodeSignalValueType = Literal[
    "PAUSE",
    "RESUME",
]
```
## PackageImportJobStatusType

```python
# PackageImportJobStatusType usage example
from types_aiobotocore_panorama.literals import PackageImportJobStatusType

def get_value() -> PackageImportJobStatusType:
    return "FAILED"
```

```python
# PackageImportJobStatusType definition
PackageImportJobStatusType = Literal[
    "FAILED",
    "PENDING",
    "SUCCEEDED",
]
```
## PackageImportJobTypeType

```python
# PackageImportJobTypeType usage example
from types_aiobotocore_panorama.literals import PackageImportJobTypeType

def get_value() -> PackageImportJobTypeType:
    return "MARKETPLACE_NODE_PACKAGE_VERSION"
```

```python
# PackageImportJobTypeType definition
PackageImportJobTypeType = Literal[
    "MARKETPLACE_NODE_PACKAGE_VERSION",
    "NODE_PACKAGE_VERSION",
]
```
## PackageVersionStatusType

```python
# PackageVersionStatusType usage example
from types_aiobotocore_panorama.literals import PackageVersionStatusType

def get_value() -> PackageVersionStatusType:
    return "DELETING"
```

```python
# PackageVersionStatusType definition
PackageVersionStatusType = Literal[
    "DELETING",
    "FAILED",
    "REGISTER_COMPLETED",
    "REGISTER_PENDING",
]
```
## PortTypeType

```python
# PortTypeType usage example
from types_aiobotocore_panorama.literals import PortTypeType

def get_value() -> PortTypeType:
    return "BOOLEAN"
```

```python
# PortTypeType definition
PortTypeType = Literal[
    "BOOLEAN",
    "FLOAT32",
    "INT32",
    "MEDIA",
    "STRING",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_panorama.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASCENDING"
```

```python
# SortOrderType definition
SortOrderType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## StatusFilterType

```python
# StatusFilterType usage example
from types_aiobotocore_panorama.literals import StatusFilterType

def get_value() -> StatusFilterType:
    return "DEPLOYMENT_ERROR"
```

```python
# StatusFilterType definition
StatusFilterType = Literal[
    "DEPLOYMENT_ERROR",
    "DEPLOYMENT_FAILED",
    "DEPLOYMENT_SUCCEEDED",
    "PROCESSING_DEPLOYMENT",
    "PROCESSING_REMOVAL",
    "REMOVAL_FAILED",
    "REMOVAL_SUCCEEDED",
]
```
## TemplateTypeType

```python
# TemplateTypeType usage example
from types_aiobotocore_panorama.literals import TemplateTypeType

def get_value() -> TemplateTypeType:
    return "RTSP_CAMERA_STREAM"
```

```python
# TemplateTypeType definition
TemplateTypeType = Literal[
    "RTSP_CAMERA_STREAM",
]
```
## UpdateProgressType

```python
# UpdateProgressType usage example
from types_aiobotocore_panorama.literals import UpdateProgressType

def get_value() -> UpdateProgressType:
    return "COMPLETED"
```

```python
# UpdateProgressType definition
UpdateProgressType = Literal[
    "COMPLETED",
    "DOWNLOADING",
    "FAILED",
    "IN_PROGRESS",
    "PENDING",
    "REBOOTING",
    "VERIFYING",
]
```
## PanoramaServiceName

```python
# PanoramaServiceName usage example
from types_aiobotocore_panorama.literals import PanoramaServiceName

def get_value() -> PanoramaServiceName:
    return "panorama"
```

```python
# PanoramaServiceName definition
PanoramaServiceName = Literal[
    "panorama",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_panorama.literals import ServiceName

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
from types_aiobotocore_panorama.literals import ResourceServiceName

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
