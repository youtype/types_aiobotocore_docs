# Literals

> [Index](../README.md) > [ACM](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## CertificateExportType

```python
# CertificateExportType usage example
from types_aiobotocore_acm.literals import CertificateExportType

def get_value() -> CertificateExportType:
    return "DISABLED"
```

```python
# CertificateExportType definition
CertificateExportType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## CertificateManagedByType

```python
# CertificateManagedByType usage example
from types_aiobotocore_acm.literals import CertificateManagedByType

def get_value() -> CertificateManagedByType:
    return "CLOUDFRONT"
```

```python
# CertificateManagedByType definition
CertificateManagedByType = Literal[
    "CLOUDFRONT",
]
```
## CertificateStatusType

```python
# CertificateStatusType usage example
from types_aiobotocore_acm.literals import CertificateStatusType

def get_value() -> CertificateStatusType:
    return "EXPIRED"
```

```python
# CertificateStatusType definition
CertificateStatusType = Literal[
    "EXPIRED",
    "FAILED",
    "INACTIVE",
    "ISSUED",
    "PENDING_VALIDATION",
    "REVOKED",
    "VALIDATION_TIMED_OUT",
]
```
## CertificateTransparencyLoggingPreferenceType

```python
# CertificateTransparencyLoggingPreferenceType usage example
from types_aiobotocore_acm.literals import CertificateTransparencyLoggingPreferenceType

def get_value() -> CertificateTransparencyLoggingPreferenceType:
    return "DISABLED"
```

```python
# CertificateTransparencyLoggingPreferenceType definition
CertificateTransparencyLoggingPreferenceType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## CertificateTypeType

```python
# CertificateTypeType usage example
from types_aiobotocore_acm.literals import CertificateTypeType

def get_value() -> CertificateTypeType:
    return "AMAZON_ISSUED"
```

```python
# CertificateTypeType definition
CertificateTypeType = Literal[
    "AMAZON_ISSUED",
    "IMPORTED",
    "PRIVATE",
]
```
## CertificateValidatedWaiterName

```python
# CertificateValidatedWaiterName usage example
from types_aiobotocore_acm.literals import CertificateValidatedWaiterName

def get_value() -> CertificateValidatedWaiterName:
    return "certificate_validated"
```

```python
# CertificateValidatedWaiterName definition
CertificateValidatedWaiterName = Literal[
    "certificate_validated",
]
```
## DomainStatusType

```python
# DomainStatusType usage example
from types_aiobotocore_acm.literals import DomainStatusType

def get_value() -> DomainStatusType:
    return "FAILED"
```

```python
# DomainStatusType definition
DomainStatusType = Literal[
    "FAILED",
    "PENDING_VALIDATION",
    "SUCCESS",
]
```
## ExtendedKeyUsageNameType

```python
# ExtendedKeyUsageNameType usage example
from types_aiobotocore_acm.literals import ExtendedKeyUsageNameType

def get_value() -> ExtendedKeyUsageNameType:
    return "ANY"
```

```python
# ExtendedKeyUsageNameType definition
ExtendedKeyUsageNameType = Literal[
    "ANY",
    "CODE_SIGNING",
    "CUSTOM",
    "EMAIL_PROTECTION",
    "IPSEC_END_SYSTEM",
    "IPSEC_TUNNEL",
    "IPSEC_USER",
    "NONE",
    "OCSP_SIGNING",
    "TIME_STAMPING",
    "TLS_WEB_CLIENT_AUTHENTICATION",
    "TLS_WEB_SERVER_AUTHENTICATION",
]
```
## FailureReasonType

```python
# FailureReasonType usage example
from types_aiobotocore_acm.literals import FailureReasonType

def get_value() -> FailureReasonType:
    return "ADDITIONAL_VERIFICATION_REQUIRED"
```

```python
# FailureReasonType definition
FailureReasonType = Literal[
    "ADDITIONAL_VERIFICATION_REQUIRED",
    "CAA_ERROR",
    "DOMAIN_NOT_ALLOWED",
    "DOMAIN_VALIDATION_DENIED",
    "INVALID_PUBLIC_DOMAIN",
    "NO_AVAILABLE_CONTACTS",
    "OTHER",
    "PCA_ACCESS_DENIED",
    "PCA_INVALID_ARGS",
    "PCA_INVALID_ARN",
    "PCA_INVALID_DURATION",
    "PCA_INVALID_STATE",
    "PCA_LIMIT_EXCEEDED",
    "PCA_NAME_CONSTRAINTS_VALIDATION",
    "PCA_REQUEST_FAILED",
    "PCA_RESOURCE_NOT_FOUND",
    "SLR_NOT_FOUND",
]
```
## KeyAlgorithmType

```python
# KeyAlgorithmType usage example
from types_aiobotocore_acm.literals import KeyAlgorithmType

def get_value() -> KeyAlgorithmType:
    return "EC_prime256v1"
```

```python
# KeyAlgorithmType definition
KeyAlgorithmType = Literal[
    "EC_prime256v1",
    "EC_secp384r1",
    "EC_secp521r1",
    "RSA_1024",
    "RSA_2048",
    "RSA_3072",
    "RSA_4096",
]
```
## KeyUsageNameType

```python
# KeyUsageNameType usage example
from types_aiobotocore_acm.literals import KeyUsageNameType

def get_value() -> KeyUsageNameType:
    return "ANY"
```

```python
# KeyUsageNameType definition
KeyUsageNameType = Literal[
    "ANY",
    "CERTIFICATE_SIGNING",
    "CRL_SIGNING",
    "CUSTOM",
    "DATA_ENCIPHERMENT",
    "DECIPHER_ONLY",
    "DIGITAL_SIGNATURE",
    "ENCIPHER_ONLY",
    "KEY_AGREEMENT",
    "KEY_ENCIPHERMENT",
    "NON_REPUDIATION",
]
```
## ListCertificatesPaginatorName

```python
# ListCertificatesPaginatorName usage example
from types_aiobotocore_acm.literals import ListCertificatesPaginatorName

def get_value() -> ListCertificatesPaginatorName:
    return "list_certificates"
```

```python
# ListCertificatesPaginatorName definition
ListCertificatesPaginatorName = Literal[
    "list_certificates",
]
```
## RecordTypeType

```python
# RecordTypeType usage example
from types_aiobotocore_acm.literals import RecordTypeType

def get_value() -> RecordTypeType:
    return "CNAME"
```

```python
# RecordTypeType definition
RecordTypeType = Literal[
    "CNAME",
]
```
## RenewalEligibilityType

```python
# RenewalEligibilityType usage example
from types_aiobotocore_acm.literals import RenewalEligibilityType

def get_value() -> RenewalEligibilityType:
    return "ELIGIBLE"
```

```python
# RenewalEligibilityType definition
RenewalEligibilityType = Literal[
    "ELIGIBLE",
    "INELIGIBLE",
]
```
## RenewalStatusType

```python
# RenewalStatusType usage example
from types_aiobotocore_acm.literals import RenewalStatusType

def get_value() -> RenewalStatusType:
    return "FAILED"
```

```python
# RenewalStatusType definition
RenewalStatusType = Literal[
    "FAILED",
    "PENDING_AUTO_RENEWAL",
    "PENDING_VALIDATION",
    "SUCCESS",
]
```
## RevocationReasonType

```python
# RevocationReasonType usage example
from types_aiobotocore_acm.literals import RevocationReasonType

def get_value() -> RevocationReasonType:
    return "AFFILIATION_CHANGED"
```

```python
# RevocationReasonType definition
RevocationReasonType = Literal[
    "A_A_COMPROMISE",
    "AFFILIATION_CHANGED",
    "CA_COMPROMISE",
    "CERTIFICATE_HOLD",
    "CESSATION_OF_OPERATION",
    "KEY_COMPROMISE",
    "PRIVILEGE_WITHDRAWN",
    "REMOVE_FROM_CRL",
    "SUPERCEDED",
    "SUPERSEDED",
    "UNSPECIFIED",
]
```
## SortByType

```python
# SortByType usage example
from types_aiobotocore_acm.literals import SortByType

def get_value() -> SortByType:
    return "CREATED_AT"
```

```python
# SortByType definition
SortByType = Literal[
    "CREATED_AT",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_acm.literals import SortOrderType

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
## ValidationMethodType

```python
# ValidationMethodType usage example
from types_aiobotocore_acm.literals import ValidationMethodType

def get_value() -> ValidationMethodType:
    return "DNS"
```

```python
# ValidationMethodType definition
ValidationMethodType = Literal[
    "DNS",
    "EMAIL",
    "HTTP",
]
```
## ACMServiceName

```python
# ACMServiceName usage example
from types_aiobotocore_acm.literals import ACMServiceName

def get_value() -> ACMServiceName:
    return "acm"
```

```python
# ACMServiceName definition
ACMServiceName = Literal[
    "acm",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_acm.literals import ServiceName

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
from types_aiobotocore_acm.literals import ResourceServiceName

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
from types_aiobotocore_acm.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_certificates"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_certificates",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_acm.literals import WaiterName

def get_value() -> WaiterName:
    return "certificate_validated"
```

```python
# WaiterName definition
WaiterName = Literal[
    "certificate_validated",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_acm.literals import RegionName

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
