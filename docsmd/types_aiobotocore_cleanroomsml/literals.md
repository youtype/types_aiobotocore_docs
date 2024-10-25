# Literals

> [Index](../README.md) > [CleanRoomsML](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## AudienceExportJobStatusType

```python
# AudienceExportJobStatusType usage example

from types_aiobotocore_cleanroomsml.literals import AudienceExportJobStatusType

def get_value() -> AudienceExportJobStatusType:
    return "ACTIVE"
```

```python
# AudienceExportJobStatusType definition

AudienceExportJobStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "CREATE_PENDING",
]
```
## AudienceGenerationJobStatusType

```python
# AudienceGenerationJobStatusType usage example

from types_aiobotocore_cleanroomsml.literals import AudienceGenerationJobStatusType

def get_value() -> AudienceGenerationJobStatusType:
    return "ACTIVE"
```

```python
# AudienceGenerationJobStatusType definition

AudienceGenerationJobStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "CREATE_PENDING",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETE_PENDING",
]
```
## AudienceModelStatusType

```python
# AudienceModelStatusType usage example

from types_aiobotocore_cleanroomsml.literals import AudienceModelStatusType

def get_value() -> AudienceModelStatusType:
    return "ACTIVE"
```

```python
# AudienceModelStatusType definition

AudienceModelStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "CREATE_PENDING",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETE_PENDING",
]
```
## AudienceSizeTypeType

```python
# AudienceSizeTypeType usage example

from types_aiobotocore_cleanroomsml.literals import AudienceSizeTypeType

def get_value() -> AudienceSizeTypeType:
    return "ABSOLUTE"
```

```python
# AudienceSizeTypeType definition

AudienceSizeTypeType = Literal[
    "ABSOLUTE",
    "PERCENTAGE",
]
```
## ColumnTypeType

```python
# ColumnTypeType usage example

from types_aiobotocore_cleanroomsml.literals import ColumnTypeType

def get_value() -> ColumnTypeType:
    return "CATEGORICAL_FEATURE"
```

```python
# ColumnTypeType definition

ColumnTypeType = Literal[
    "CATEGORICAL_FEATURE",
    "ITEM_ID",
    "NUMERICAL_FEATURE",
    "TIMESTAMP",
    "USER_ID",
]
```
## ConfiguredAudienceModelStatusType

```python
# ConfiguredAudienceModelStatusType usage example

from types_aiobotocore_cleanroomsml.literals import ConfiguredAudienceModelStatusType

def get_value() -> ConfiguredAudienceModelStatusType:
    return "ACTIVE"
```

```python
# ConfiguredAudienceModelStatusType definition

ConfiguredAudienceModelStatusType = Literal[
    "ACTIVE",
]
```
## DatasetTypeType

```python
# DatasetTypeType usage example

from types_aiobotocore_cleanroomsml.literals import DatasetTypeType

def get_value() -> DatasetTypeType:
    return "INTERACTIONS"
```

```python
# DatasetTypeType definition

DatasetTypeType = Literal[
    "INTERACTIONS",
]
```
## ListAudienceExportJobsPaginatorName

```python
# ListAudienceExportJobsPaginatorName usage example

from types_aiobotocore_cleanroomsml.literals import ListAudienceExportJobsPaginatorName

def get_value() -> ListAudienceExportJobsPaginatorName:
    return "list_audience_export_jobs"
```

```python
# ListAudienceExportJobsPaginatorName definition

ListAudienceExportJobsPaginatorName = Literal[
    "list_audience_export_jobs",
]
```
## ListAudienceGenerationJobsPaginatorName

```python
# ListAudienceGenerationJobsPaginatorName usage example

from types_aiobotocore_cleanroomsml.literals import ListAudienceGenerationJobsPaginatorName

def get_value() -> ListAudienceGenerationJobsPaginatorName:
    return "list_audience_generation_jobs"
```

```python
# ListAudienceGenerationJobsPaginatorName definition

ListAudienceGenerationJobsPaginatorName = Literal[
    "list_audience_generation_jobs",
]
```
## ListAudienceModelsPaginatorName

```python
# ListAudienceModelsPaginatorName usage example

from types_aiobotocore_cleanroomsml.literals import ListAudienceModelsPaginatorName

def get_value() -> ListAudienceModelsPaginatorName:
    return "list_audience_models"
```

```python
# ListAudienceModelsPaginatorName definition

ListAudienceModelsPaginatorName = Literal[
    "list_audience_models",
]
```
## ListConfiguredAudienceModelsPaginatorName

```python
# ListConfiguredAudienceModelsPaginatorName usage example

from types_aiobotocore_cleanroomsml.literals import ListConfiguredAudienceModelsPaginatorName

def get_value() -> ListConfiguredAudienceModelsPaginatorName:
    return "list_configured_audience_models"
```

```python
# ListConfiguredAudienceModelsPaginatorName definition

ListConfiguredAudienceModelsPaginatorName = Literal[
    "list_configured_audience_models",
]
```
## ListTrainingDatasetsPaginatorName

```python
# ListTrainingDatasetsPaginatorName usage example

from types_aiobotocore_cleanroomsml.literals import ListTrainingDatasetsPaginatorName

def get_value() -> ListTrainingDatasetsPaginatorName:
    return "list_training_datasets"
```

```python
# ListTrainingDatasetsPaginatorName definition

ListTrainingDatasetsPaginatorName = Literal[
    "list_training_datasets",
]
```
## PolicyExistenceConditionType

```python
# PolicyExistenceConditionType usage example

from types_aiobotocore_cleanroomsml.literals import PolicyExistenceConditionType

def get_value() -> PolicyExistenceConditionType:
    return "POLICY_MUST_EXIST"
```

```python
# PolicyExistenceConditionType definition

PolicyExistenceConditionType = Literal[
    "POLICY_MUST_EXIST",
    "POLICY_MUST_NOT_EXIST",
]
```
## SharedAudienceMetricsType

```python
# SharedAudienceMetricsType usage example

from types_aiobotocore_cleanroomsml.literals import SharedAudienceMetricsType

def get_value() -> SharedAudienceMetricsType:
    return "ALL"
```

```python
# SharedAudienceMetricsType definition

SharedAudienceMetricsType = Literal[
    "ALL",
    "NONE",
]
```
## TagOnCreatePolicyType

```python
# TagOnCreatePolicyType usage example

from types_aiobotocore_cleanroomsml.literals import TagOnCreatePolicyType

def get_value() -> TagOnCreatePolicyType:
    return "FROM_PARENT_RESOURCE"
```

```python
# TagOnCreatePolicyType definition

TagOnCreatePolicyType = Literal[
    "FROM_PARENT_RESOURCE",
    "NONE",
]
```
## TrainingDatasetStatusType

```python
# TrainingDatasetStatusType usage example

from types_aiobotocore_cleanroomsml.literals import TrainingDatasetStatusType

def get_value() -> TrainingDatasetStatusType:
    return "ACTIVE"
```

```python
# TrainingDatasetStatusType definition

TrainingDatasetStatusType = Literal[
    "ACTIVE",
]
```
## CleanRoomsMLServiceName

```python
# CleanRoomsMLServiceName usage example

from types_aiobotocore_cleanroomsml.literals import CleanRoomsMLServiceName

def get_value() -> CleanRoomsMLServiceName:
    return "cleanroomsml"
```

```python
# CleanRoomsMLServiceName definition

CleanRoomsMLServiceName = Literal[
    "cleanroomsml",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_cleanroomsml.literals import ServiceName

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
    "batch",
    "bcm-data-exports",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-runtime",
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
    "iot",
    "iot-data",
    "iot-jobs-data",
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
    "networkmanager",
    "networkmonitor",
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

from types_aiobotocore_cleanroomsml.literals import ResourceServiceName

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

from types_aiobotocore_cleanroomsml.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_audience_export_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_audience_export_jobs",
    "list_audience_generation_jobs",
    "list_audience_models",
    "list_configured_audience_models",
    "list_training_datasets",
]
```
