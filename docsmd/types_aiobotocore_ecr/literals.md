# Literals

> [Index](../README.md) > [ECR](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## DescribeImageScanFindingsPaginatorName

```python
# DescribeImageScanFindingsPaginatorName usage example
from types_aiobotocore_ecr.literals import DescribeImageScanFindingsPaginatorName

def get_value() -> DescribeImageScanFindingsPaginatorName:
    return "describe_image_scan_findings"
```

```python
# DescribeImageScanFindingsPaginatorName definition
DescribeImageScanFindingsPaginatorName = Literal[
    "describe_image_scan_findings",
]
```
## DescribeImagesPaginatorName

```python
# DescribeImagesPaginatorName usage example
from types_aiobotocore_ecr.literals import DescribeImagesPaginatorName

def get_value() -> DescribeImagesPaginatorName:
    return "describe_images"
```

```python
# DescribeImagesPaginatorName definition
DescribeImagesPaginatorName = Literal[
    "describe_images",
]
```
## DescribePullThroughCacheRulesPaginatorName

```python
# DescribePullThroughCacheRulesPaginatorName usage example
from types_aiobotocore_ecr.literals import DescribePullThroughCacheRulesPaginatorName

def get_value() -> DescribePullThroughCacheRulesPaginatorName:
    return "describe_pull_through_cache_rules"
```

```python
# DescribePullThroughCacheRulesPaginatorName definition
DescribePullThroughCacheRulesPaginatorName = Literal[
    "describe_pull_through_cache_rules",
]
```
## DescribeRepositoriesPaginatorName

```python
# DescribeRepositoriesPaginatorName usage example
from types_aiobotocore_ecr.literals import DescribeRepositoriesPaginatorName

def get_value() -> DescribeRepositoriesPaginatorName:
    return "describe_repositories"
```

```python
# DescribeRepositoriesPaginatorName definition
DescribeRepositoriesPaginatorName = Literal[
    "describe_repositories",
]
```
## DescribeRepositoryCreationTemplatesPaginatorName

```python
# DescribeRepositoryCreationTemplatesPaginatorName usage example
from types_aiobotocore_ecr.literals import DescribeRepositoryCreationTemplatesPaginatorName

def get_value() -> DescribeRepositoryCreationTemplatesPaginatorName:
    return "describe_repository_creation_templates"
```

```python
# DescribeRepositoryCreationTemplatesPaginatorName definition
DescribeRepositoryCreationTemplatesPaginatorName = Literal[
    "describe_repository_creation_templates",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example
from types_aiobotocore_ecr.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "AES256"
```

```python
# EncryptionTypeType definition
EncryptionTypeType = Literal[
    "AES256",
    "KMS",
    "KMS_DSSE",
]
```
## FindingSeverityType

```python
# FindingSeverityType usage example
from types_aiobotocore_ecr.literals import FindingSeverityType

def get_value() -> FindingSeverityType:
    return "CRITICAL"
```

```python
# FindingSeverityType definition
FindingSeverityType = Literal[
    "CRITICAL",
    "HIGH",
    "INFORMATIONAL",
    "LOW",
    "MEDIUM",
    "UNDEFINED",
]
```
## GetLifecyclePolicyPreviewPaginatorName

```python
# GetLifecyclePolicyPreviewPaginatorName usage example
from types_aiobotocore_ecr.literals import GetLifecyclePolicyPreviewPaginatorName

def get_value() -> GetLifecyclePolicyPreviewPaginatorName:
    return "get_lifecycle_policy_preview"
```

```python
# GetLifecyclePolicyPreviewPaginatorName definition
GetLifecyclePolicyPreviewPaginatorName = Literal[
    "get_lifecycle_policy_preview",
]
```
## ImageActionTypeType

```python
# ImageActionTypeType usage example
from types_aiobotocore_ecr.literals import ImageActionTypeType

def get_value() -> ImageActionTypeType:
    return "EXPIRE"
```

```python
# ImageActionTypeType definition
ImageActionTypeType = Literal[
    "EXPIRE",
]
```
## ImageFailureCodeType

```python
# ImageFailureCodeType usage example
from types_aiobotocore_ecr.literals import ImageFailureCodeType

def get_value() -> ImageFailureCodeType:
    return "ImageNotFound"
```

```python
# ImageFailureCodeType definition
ImageFailureCodeType = Literal[
    "ImageNotFound",
    "ImageReferencedByManifestList",
    "ImageTagDoesNotMatchDigest",
    "InvalidImageDigest",
    "InvalidImageTag",
    "KmsError",
    "MissingDigestAndTag",
    "UpstreamAccessDenied",
    "UpstreamTooManyRequests",
    "UpstreamUnavailable",
]
```
## ImageScanCompleteWaiterName

```python
# ImageScanCompleteWaiterName usage example
from types_aiobotocore_ecr.literals import ImageScanCompleteWaiterName

def get_value() -> ImageScanCompleteWaiterName:
    return "image_scan_complete"
```

```python
# ImageScanCompleteWaiterName definition
ImageScanCompleteWaiterName = Literal[
    "image_scan_complete",
]
```
## ImageTagMutabilityType

```python
# ImageTagMutabilityType usage example
from types_aiobotocore_ecr.literals import ImageTagMutabilityType

def get_value() -> ImageTagMutabilityType:
    return "IMMUTABLE"
```

```python
# ImageTagMutabilityType definition
ImageTagMutabilityType = Literal[
    "IMMUTABLE",
    "MUTABLE",
]
```
## LayerAvailabilityType

```python
# LayerAvailabilityType usage example
from types_aiobotocore_ecr.literals import LayerAvailabilityType

def get_value() -> LayerAvailabilityType:
    return "AVAILABLE"
```

```python
# LayerAvailabilityType definition
LayerAvailabilityType = Literal[
    "AVAILABLE",
    "UNAVAILABLE",
]
```
## LayerFailureCodeType

```python
# LayerFailureCodeType usage example
from types_aiobotocore_ecr.literals import LayerFailureCodeType

def get_value() -> LayerFailureCodeType:
    return "InvalidLayerDigest"
```

```python
# LayerFailureCodeType definition
LayerFailureCodeType = Literal[
    "InvalidLayerDigest",
    "MissingLayerDigest",
]
```
## LifecyclePolicyPreviewCompleteWaiterName

```python
# LifecyclePolicyPreviewCompleteWaiterName usage example
from types_aiobotocore_ecr.literals import LifecyclePolicyPreviewCompleteWaiterName

def get_value() -> LifecyclePolicyPreviewCompleteWaiterName:
    return "lifecycle_policy_preview_complete"
```

```python
# LifecyclePolicyPreviewCompleteWaiterName definition
LifecyclePolicyPreviewCompleteWaiterName = Literal[
    "lifecycle_policy_preview_complete",
]
```
## LifecyclePolicyPreviewStatusType

```python
# LifecyclePolicyPreviewStatusType usage example
from types_aiobotocore_ecr.literals import LifecyclePolicyPreviewStatusType

def get_value() -> LifecyclePolicyPreviewStatusType:
    return "COMPLETE"
```

```python
# LifecyclePolicyPreviewStatusType definition
LifecyclePolicyPreviewStatusType = Literal[
    "COMPLETE",
    "EXPIRED",
    "FAILED",
    "IN_PROGRESS",
]
```
## ListImagesPaginatorName

```python
# ListImagesPaginatorName usage example
from types_aiobotocore_ecr.literals import ListImagesPaginatorName

def get_value() -> ListImagesPaginatorName:
    return "list_images"
```

```python
# ListImagesPaginatorName definition
ListImagesPaginatorName = Literal[
    "list_images",
]
```
## RCTAppliedForType

```python
# RCTAppliedForType usage example
from types_aiobotocore_ecr.literals import RCTAppliedForType

def get_value() -> RCTAppliedForType:
    return "PULL_THROUGH_CACHE"
```

```python
# RCTAppliedForType definition
RCTAppliedForType = Literal[
    "PULL_THROUGH_CACHE",
    "REPLICATION",
]
```
## ReplicationStatusType

```python
# ReplicationStatusType usage example
from types_aiobotocore_ecr.literals import ReplicationStatusType

def get_value() -> ReplicationStatusType:
    return "COMPLETE"
```

```python
# ReplicationStatusType definition
ReplicationStatusType = Literal[
    "COMPLETE",
    "FAILED",
    "IN_PROGRESS",
]
```
## RepositoryFilterTypeType

```python
# RepositoryFilterTypeType usage example
from types_aiobotocore_ecr.literals import RepositoryFilterTypeType

def get_value() -> RepositoryFilterTypeType:
    return "PREFIX_MATCH"
```

```python
# RepositoryFilterTypeType definition
RepositoryFilterTypeType = Literal[
    "PREFIX_MATCH",
]
```
## ScanFrequencyType

```python
# ScanFrequencyType usage example
from types_aiobotocore_ecr.literals import ScanFrequencyType

def get_value() -> ScanFrequencyType:
    return "CONTINUOUS_SCAN"
```

```python
# ScanFrequencyType definition
ScanFrequencyType = Literal[
    "CONTINUOUS_SCAN",
    "MANUAL",
    "SCAN_ON_PUSH",
]
```
## ScanStatusType

```python
# ScanStatusType usage example
from types_aiobotocore_ecr.literals import ScanStatusType

def get_value() -> ScanStatusType:
    return "ACTIVE"
```

```python
# ScanStatusType definition
ScanStatusType = Literal[
    "ACTIVE",
    "COMPLETE",
    "FAILED",
    "FINDINGS_UNAVAILABLE",
    "IN_PROGRESS",
    "LIMIT_EXCEEDED",
    "PENDING",
    "SCAN_ELIGIBILITY_EXPIRED",
    "UNSUPPORTED_IMAGE",
]
```
## ScanTypeType

```python
# ScanTypeType usage example
from types_aiobotocore_ecr.literals import ScanTypeType

def get_value() -> ScanTypeType:
    return "BASIC"
```

```python
# ScanTypeType definition
ScanTypeType = Literal[
    "BASIC",
    "ENHANCED",
]
```
## ScanningConfigurationFailureCodeType

```python
# ScanningConfigurationFailureCodeType usage example
from types_aiobotocore_ecr.literals import ScanningConfigurationFailureCodeType

def get_value() -> ScanningConfigurationFailureCodeType:
    return "REPOSITORY_NOT_FOUND"
```

```python
# ScanningConfigurationFailureCodeType definition
ScanningConfigurationFailureCodeType = Literal[
    "REPOSITORY_NOT_FOUND",
]
```
## ScanningRepositoryFilterTypeType

```python
# ScanningRepositoryFilterTypeType usage example
from types_aiobotocore_ecr.literals import ScanningRepositoryFilterTypeType

def get_value() -> ScanningRepositoryFilterTypeType:
    return "WILDCARD"
```

```python
# ScanningRepositoryFilterTypeType definition
ScanningRepositoryFilterTypeType = Literal[
    "WILDCARD",
]
```
## TagStatusType

```python
# TagStatusType usage example
from types_aiobotocore_ecr.literals import TagStatusType

def get_value() -> TagStatusType:
    return "ANY"
```

```python
# TagStatusType definition
TagStatusType = Literal[
    "ANY",
    "TAGGED",
    "UNTAGGED",
]
```
## UpstreamRegistryType

```python
# UpstreamRegistryType usage example
from types_aiobotocore_ecr.literals import UpstreamRegistryType

def get_value() -> UpstreamRegistryType:
    return "azure-container-registry"
```

```python
# UpstreamRegistryType definition
UpstreamRegistryType = Literal[
    "azure-container-registry",
    "docker-hub",
    "ecr-public",
    "github-container-registry",
    "gitlab-container-registry",
    "k8s",
    "quay",
]
```
## ECRServiceName

```python
# ECRServiceName usage example
from types_aiobotocore_ecr.literals import ECRServiceName

def get_value() -> ECRServiceName:
    return "ecr"
```

```python
# ECRServiceName definition
ECRServiceName = Literal[
    "ecr",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_ecr.literals import ServiceName

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
from types_aiobotocore_ecr.literals import ResourceServiceName

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
from types_aiobotocore_ecr.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_image_scan_findings"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_image_scan_findings",
    "describe_images",
    "describe_pull_through_cache_rules",
    "describe_repositories",
    "describe_repository_creation_templates",
    "get_lifecycle_policy_preview",
    "list_images",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_ecr.literals import WaiterName

def get_value() -> WaiterName:
    return "image_scan_complete"
```

```python
# WaiterName definition
WaiterName = Literal[
    "image_scan_complete",
    "lifecycle_policy_preview_complete",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_ecr.literals import RegionName

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
