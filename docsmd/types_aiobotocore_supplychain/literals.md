# Literals

> [Index](../README.md) > [SupplyChain](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## ConfigurationJobStatusType

```python
# ConfigurationJobStatusType usage example
from types_aiobotocore_supplychain.literals import ConfigurationJobStatusType

def get_value() -> ConfigurationJobStatusType:
    return "FAILED"
```

```python
# ConfigurationJobStatusType definition
ConfigurationJobStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "NEW",
    "QUEUED",
    "SUCCESS",
]
```
## DataIntegrationEventTypeType

```python
# DataIntegrationEventTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationEventTypeType

def get_value() -> DataIntegrationEventTypeType:
    return "scn.data.forecast"
```

```python
# DataIntegrationEventTypeType definition
DataIntegrationEventTypeType = Literal[
    "scn.data.forecast",
    "scn.data.inboundorder",
    "scn.data.inboundorderline",
    "scn.data.inboundorderlineschedule",
    "scn.data.inventorylevel",
    "scn.data.outboundorderline",
    "scn.data.outboundshipment",
    "scn.data.processheader",
    "scn.data.processoperation",
    "scn.data.processproduct",
    "scn.data.reservation",
    "scn.data.shipment",
    "scn.data.shipmentstop",
    "scn.data.shipmentstoporder",
    "scn.data.supplyplan",
]
```
## DataIntegrationFlowFileTypeType

```python
# DataIntegrationFlowFileTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationFlowFileTypeType

def get_value() -> DataIntegrationFlowFileTypeType:
    return "CSV"
```

```python
# DataIntegrationFlowFileTypeType definition
DataIntegrationFlowFileTypeType = Literal[
    "CSV",
    "JSON",
    "PARQUET",
]
```
## DataIntegrationFlowLoadTypeType

```python
# DataIntegrationFlowLoadTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationFlowLoadTypeType

def get_value() -> DataIntegrationFlowLoadTypeType:
    return "INCREMENTAL"
```

```python
# DataIntegrationFlowLoadTypeType definition
DataIntegrationFlowLoadTypeType = Literal[
    "INCREMENTAL",
    "REPLACE",
]
```
## DataIntegrationFlowSourceTypeType

```python
# DataIntegrationFlowSourceTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationFlowSourceTypeType

def get_value() -> DataIntegrationFlowSourceTypeType:
    return "DATASET"
```

```python
# DataIntegrationFlowSourceTypeType definition
DataIntegrationFlowSourceTypeType = Literal[
    "DATASET",
    "S3",
]
```
## DataIntegrationFlowTargetTypeType

```python
# DataIntegrationFlowTargetTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationFlowTargetTypeType

def get_value() -> DataIntegrationFlowTargetTypeType:
    return "DATASET"
```

```python
# DataIntegrationFlowTargetTypeType definition
DataIntegrationFlowTargetTypeType = Literal[
    "DATASET",
    "S3",
]
```
## DataIntegrationFlowTransformationTypeType

```python
# DataIntegrationFlowTransformationTypeType usage example
from types_aiobotocore_supplychain.literals import DataIntegrationFlowTransformationTypeType

def get_value() -> DataIntegrationFlowTransformationTypeType:
    return "NONE"
```

```python
# DataIntegrationFlowTransformationTypeType definition
DataIntegrationFlowTransformationTypeType = Literal[
    "NONE",
    "SQL",
]
```
## DataLakeDatasetSchemaFieldTypeType

```python
# DataLakeDatasetSchemaFieldTypeType usage example
from types_aiobotocore_supplychain.literals import DataLakeDatasetSchemaFieldTypeType

def get_value() -> DataLakeDatasetSchemaFieldTypeType:
    return "DOUBLE"
```

```python
# DataLakeDatasetSchemaFieldTypeType definition
DataLakeDatasetSchemaFieldTypeType = Literal[
    "DOUBLE",
    "INT",
    "STRING",
    "TIMESTAMP",
]
```
## InstanceStateType

```python
# InstanceStateType usage example
from types_aiobotocore_supplychain.literals import InstanceStateType

def get_value() -> InstanceStateType:
    return "Active"
```

```python
# InstanceStateType definition
InstanceStateType = Literal[
    "Active",
    "CreateFailed",
    "Deleted",
    "DeleteFailed",
    "Deleting",
    "Initializing",
]
```
## ListDataIntegrationFlowsPaginatorName

```python
# ListDataIntegrationFlowsPaginatorName usage example
from types_aiobotocore_supplychain.literals import ListDataIntegrationFlowsPaginatorName

def get_value() -> ListDataIntegrationFlowsPaginatorName:
    return "list_data_integration_flows"
```

```python
# ListDataIntegrationFlowsPaginatorName definition
ListDataIntegrationFlowsPaginatorName = Literal[
    "list_data_integration_flows",
]
```
## ListDataLakeDatasetsPaginatorName

```python
# ListDataLakeDatasetsPaginatorName usage example
from types_aiobotocore_supplychain.literals import ListDataLakeDatasetsPaginatorName

def get_value() -> ListDataLakeDatasetsPaginatorName:
    return "list_data_lake_datasets"
```

```python
# ListDataLakeDatasetsPaginatorName definition
ListDataLakeDatasetsPaginatorName = Literal[
    "list_data_lake_datasets",
]
```
## ListInstancesPaginatorName

```python
# ListInstancesPaginatorName usage example
from types_aiobotocore_supplychain.literals import ListInstancesPaginatorName

def get_value() -> ListInstancesPaginatorName:
    return "list_instances"
```

```python
# ListInstancesPaginatorName definition
ListInstancesPaginatorName = Literal[
    "list_instances",
]
```
## SupplyChainServiceName

```python
# SupplyChainServiceName usage example
from types_aiobotocore_supplychain.literals import SupplyChainServiceName

def get_value() -> SupplyChainServiceName:
    return "supplychain"
```

```python
# SupplyChainServiceName definition
SupplyChainServiceName = Literal[
    "supplychain",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_supplychain.literals import ServiceName

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
from types_aiobotocore_supplychain.literals import ResourceServiceName

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
from types_aiobotocore_supplychain.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_data_integration_flows"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_data_integration_flows",
    "list_data_lake_datasets",
    "list_instances",
]
```
