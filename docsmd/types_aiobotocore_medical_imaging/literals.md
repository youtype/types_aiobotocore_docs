# Literals

> [Index](../README.md) > [HealthImaging](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

## DatastoreStatusType

```python
# DatastoreStatusType usage example
from types_aiobotocore_medical_imaging.literals import DatastoreStatusType

def get_value() -> DatastoreStatusType:
    return "ACTIVE"
```

```python
# DatastoreStatusType definition
DatastoreStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETED",
    "DELETING",
]
```
## ImageSetStateType

```python
# ImageSetStateType usage example
from types_aiobotocore_medical_imaging.literals import ImageSetStateType

def get_value() -> ImageSetStateType:
    return "ACTIVE"
```

```python
# ImageSetStateType definition
ImageSetStateType = Literal[
    "ACTIVE",
    "DELETED",
    "LOCKED",
]
```
## ImageSetWorkflowStatusType

```python
# ImageSetWorkflowStatusType usage example
from types_aiobotocore_medical_imaging.literals import ImageSetWorkflowStatusType

def get_value() -> ImageSetWorkflowStatusType:
    return "COPIED"
```

```python
# ImageSetWorkflowStatusType definition
ImageSetWorkflowStatusType = Literal[
    "COPIED",
    "COPY_FAILED",
    "COPYING",
    "COPYING_WITH_READ_ONLY_ACCESS",
    "CREATED",
    "DELETED",
    "DELETING",
    "IMPORT_FAILED",
    "IMPORTED",
    "IMPORTING",
    "UPDATE_FAILED",
    "UPDATED",
    "UPDATING",
]
```
## JobStatusType

```python
# JobStatusType usage example
from types_aiobotocore_medical_imaging.literals import JobStatusType

def get_value() -> JobStatusType:
    return "COMPLETED"
```

```python
# JobStatusType definition
JobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "SUBMITTED",
]
```
## ListDICOMImportJobsPaginatorName

```python
# ListDICOMImportJobsPaginatorName usage example
from types_aiobotocore_medical_imaging.literals import ListDICOMImportJobsPaginatorName

def get_value() -> ListDICOMImportJobsPaginatorName:
    return "list_dicom_import_jobs"
```

```python
# ListDICOMImportJobsPaginatorName definition
ListDICOMImportJobsPaginatorName = Literal[
    "list_dicom_import_jobs",
]
```
## ListDatastoresPaginatorName

```python
# ListDatastoresPaginatorName usage example
from types_aiobotocore_medical_imaging.literals import ListDatastoresPaginatorName

def get_value() -> ListDatastoresPaginatorName:
    return "list_datastores"
```

```python
# ListDatastoresPaginatorName definition
ListDatastoresPaginatorName = Literal[
    "list_datastores",
]
```
## ListImageSetVersionsPaginatorName

```python
# ListImageSetVersionsPaginatorName usage example
from types_aiobotocore_medical_imaging.literals import ListImageSetVersionsPaginatorName

def get_value() -> ListImageSetVersionsPaginatorName:
    return "list_image_set_versions"
```

```python
# ListImageSetVersionsPaginatorName definition
ListImageSetVersionsPaginatorName = Literal[
    "list_image_set_versions",
]
```
## LosslessStorageFormatType

```python
# LosslessStorageFormatType usage example
from types_aiobotocore_medical_imaging.literals import LosslessStorageFormatType

def get_value() -> LosslessStorageFormatType:
    return "HTJ2K"
```

```python
# LosslessStorageFormatType definition
LosslessStorageFormatType = Literal[
    "HTJ2K",
    "JPEG_2000_LOSSLESS",
]
```
## OperatorType

```python
# OperatorType usage example
from types_aiobotocore_medical_imaging.literals import OperatorType

def get_value() -> OperatorType:
    return "BETWEEN"
```

```python
# OperatorType definition
OperatorType = Literal[
    "BETWEEN",
    "EQUAL",
]
```
## SearchImageSetsPaginatorName

```python
# SearchImageSetsPaginatorName usage example
from types_aiobotocore_medical_imaging.literals import SearchImageSetsPaginatorName

def get_value() -> SearchImageSetsPaginatorName:
    return "search_image_sets"
```

```python
# SearchImageSetsPaginatorName definition
SearchImageSetsPaginatorName = Literal[
    "search_image_sets",
]
```
## SortFieldType

```python
# SortFieldType usage example
from types_aiobotocore_medical_imaging.literals import SortFieldType

def get_value() -> SortFieldType:
    return "DICOMStudyDateAndTime"
```

```python
# SortFieldType definition
SortFieldType = Literal[
    "createdAt",
    "DICOMStudyDateAndTime",
    "updatedAt",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_medical_imaging.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASC"
```

```python
# SortOrderType definition
SortOrderType = Literal[
    "ASC",
    "DESC",
]
```
## StorageTierType

```python
# StorageTierType usage example
from types_aiobotocore_medical_imaging.literals import StorageTierType

def get_value() -> StorageTierType:
    return "ARCHIVE_INSTANT_ACCESS"
```

```python
# StorageTierType definition
StorageTierType = Literal[
    "ARCHIVE_INSTANT_ACCESS",
    "FREQUENT_ACCESS",
]
```
## HealthImagingServiceName

```python
# HealthImagingServiceName usage example
from types_aiobotocore_medical_imaging.literals import HealthImagingServiceName

def get_value() -> HealthImagingServiceName:
    return "medical-imaging"
```

```python
# HealthImagingServiceName definition
HealthImagingServiceName = Literal[
    "medical-imaging",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_medical_imaging.literals import ServiceName

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
from types_aiobotocore_medical_imaging.literals import ResourceServiceName

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
from types_aiobotocore_medical_imaging.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_datastores"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_datastores",
    "list_dicom_import_jobs",
    "list_image_set_versions",
    "search_image_sets",
]
```
