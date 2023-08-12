# Literals

> [Index](../README.md) > [Transfer](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## AgreementStatusTypeType

```python
# AgreementStatusTypeType usage example

from types_aiobotocore_transfer.literals import AgreementStatusTypeType

def get_value() -> AgreementStatusTypeType:
    return "ACTIVE"
```

```python
# AgreementStatusTypeType definition

AgreementStatusTypeType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## As2TransportType

```python
# As2TransportType usage example

from types_aiobotocore_transfer.literals import As2TransportType

def get_value() -> As2TransportType:
    return "HTTP"
```

```python
# As2TransportType definition

As2TransportType = Literal[
    "HTTP",
]
```
## CertificateStatusTypeType

```python
# CertificateStatusTypeType usage example

from types_aiobotocore_transfer.literals import CertificateStatusTypeType

def get_value() -> CertificateStatusTypeType:
    return "ACTIVE"
```

```python
# CertificateStatusTypeType definition

CertificateStatusTypeType = Literal[
    "ACTIVE",
    "INACTIVE",
    "PENDING_ROTATION",
]
```
## CertificateTypeType

```python
# CertificateTypeType usage example

from types_aiobotocore_transfer.literals import CertificateTypeType

def get_value() -> CertificateTypeType:
    return "CERTIFICATE"
```

```python
# CertificateTypeType definition

CertificateTypeType = Literal[
    "CERTIFICATE",
    "CERTIFICATE_WITH_PRIVATE_KEY",
]
```
## CertificateUsageTypeType

```python
# CertificateUsageTypeType usage example

from types_aiobotocore_transfer.literals import CertificateUsageTypeType

def get_value() -> CertificateUsageTypeType:
    return "ENCRYPTION"
```

```python
# CertificateUsageTypeType definition

CertificateUsageTypeType = Literal[
    "ENCRYPTION",
    "SIGNING",
]
```
## CompressionEnumType

```python
# CompressionEnumType usage example

from types_aiobotocore_transfer.literals import CompressionEnumType

def get_value() -> CompressionEnumType:
    return "DISABLED"
```

```python
# CompressionEnumType definition

CompressionEnumType = Literal[
    "DISABLED",
    "ZLIB",
]
```
## CustomStepStatusType

```python
# CustomStepStatusType usage example

from types_aiobotocore_transfer.literals import CustomStepStatusType

def get_value() -> CustomStepStatusType:
    return "FAILURE"
```

```python
# CustomStepStatusType definition

CustomStepStatusType = Literal[
    "FAILURE",
    "SUCCESS",
]
```
## DomainType

```python
# DomainType usage example

from types_aiobotocore_transfer.literals import DomainType

def get_value() -> DomainType:
    return "EFS"
```

```python
# DomainType definition

DomainType = Literal[
    "EFS",
    "S3",
]
```
## EncryptionAlgType

```python
# EncryptionAlgType usage example

from types_aiobotocore_transfer.literals import EncryptionAlgType

def get_value() -> EncryptionAlgType:
    return "AES128_CBC"
```

```python
# EncryptionAlgType definition

EncryptionAlgType = Literal[
    "AES128_CBC",
    "AES192_CBC",
    "AES256_CBC",
    "NONE",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example

from types_aiobotocore_transfer.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "PGP"
```

```python
# EncryptionTypeType definition

EncryptionTypeType = Literal[
    "PGP",
]
```
## EndpointTypeType

```python
# EndpointTypeType usage example

from types_aiobotocore_transfer.literals import EndpointTypeType

def get_value() -> EndpointTypeType:
    return "PUBLIC"
```

```python
# EndpointTypeType definition

EndpointTypeType = Literal[
    "PUBLIC",
    "VPC",
    "VPC_ENDPOINT",
]
```
## ExecutionErrorTypeType

```python
# ExecutionErrorTypeType usage example

from types_aiobotocore_transfer.literals import ExecutionErrorTypeType

def get_value() -> ExecutionErrorTypeType:
    return "ALREADY_EXISTS"
```

```python
# ExecutionErrorTypeType definition

ExecutionErrorTypeType = Literal[
    "ALREADY_EXISTS",
    "BAD_REQUEST",
    "CUSTOM_STEP_FAILED",
    "INTERNAL_SERVER_ERROR",
    "NOT_FOUND",
    "PERMISSION_DENIED",
    "THROTTLED",
    "TIMEOUT",
]
```
## ExecutionStatusType

```python
# ExecutionStatusType usage example

from types_aiobotocore_transfer.literals import ExecutionStatusType

def get_value() -> ExecutionStatusType:
    return "COMPLETED"
```

```python
# ExecutionStatusType definition

ExecutionStatusType = Literal[
    "COMPLETED",
    "EXCEPTION",
    "HANDLING_EXCEPTION",
    "IN_PROGRESS",
]
```
## HomeDirectoryTypeType

```python
# HomeDirectoryTypeType usage example

from types_aiobotocore_transfer.literals import HomeDirectoryTypeType

def get_value() -> HomeDirectoryTypeType:
    return "LOGICAL"
```

```python
# HomeDirectoryTypeType definition

HomeDirectoryTypeType = Literal[
    "LOGICAL",
    "PATH",
]
```
## IdentityProviderTypeType

```python
# IdentityProviderTypeType usage example

from types_aiobotocore_transfer.literals import IdentityProviderTypeType

def get_value() -> IdentityProviderTypeType:
    return "API_GATEWAY"
```

```python
# IdentityProviderTypeType definition

IdentityProviderTypeType = Literal[
    "API_GATEWAY",
    "AWS_DIRECTORY_SERVICE",
    "AWS_LAMBDA",
    "SERVICE_MANAGED",
]
```
## ListAccessesPaginatorName

```python
# ListAccessesPaginatorName usage example

from types_aiobotocore_transfer.literals import ListAccessesPaginatorName

def get_value() -> ListAccessesPaginatorName:
    return "list_accesses"
```

```python
# ListAccessesPaginatorName definition

ListAccessesPaginatorName = Literal[
    "list_accesses",
]
```
## ListAgreementsPaginatorName

```python
# ListAgreementsPaginatorName usage example

from types_aiobotocore_transfer.literals import ListAgreementsPaginatorName

def get_value() -> ListAgreementsPaginatorName:
    return "list_agreements"
```

```python
# ListAgreementsPaginatorName definition

ListAgreementsPaginatorName = Literal[
    "list_agreements",
]
```
## ListCertificatesPaginatorName

```python
# ListCertificatesPaginatorName usage example

from types_aiobotocore_transfer.literals import ListCertificatesPaginatorName

def get_value() -> ListCertificatesPaginatorName:
    return "list_certificates"
```

```python
# ListCertificatesPaginatorName definition

ListCertificatesPaginatorName = Literal[
    "list_certificates",
]
```
## ListConnectorsPaginatorName

```python
# ListConnectorsPaginatorName usage example

from types_aiobotocore_transfer.literals import ListConnectorsPaginatorName

def get_value() -> ListConnectorsPaginatorName:
    return "list_connectors"
```

```python
# ListConnectorsPaginatorName definition

ListConnectorsPaginatorName = Literal[
    "list_connectors",
]
```
## ListExecutionsPaginatorName

```python
# ListExecutionsPaginatorName usage example

from types_aiobotocore_transfer.literals import ListExecutionsPaginatorName

def get_value() -> ListExecutionsPaginatorName:
    return "list_executions"
```

```python
# ListExecutionsPaginatorName definition

ListExecutionsPaginatorName = Literal[
    "list_executions",
]
```
## ListProfilesPaginatorName

```python
# ListProfilesPaginatorName usage example

from types_aiobotocore_transfer.literals import ListProfilesPaginatorName

def get_value() -> ListProfilesPaginatorName:
    return "list_profiles"
```

```python
# ListProfilesPaginatorName definition

ListProfilesPaginatorName = Literal[
    "list_profiles",
]
```
## ListSecurityPoliciesPaginatorName

```python
# ListSecurityPoliciesPaginatorName usage example

from types_aiobotocore_transfer.literals import ListSecurityPoliciesPaginatorName

def get_value() -> ListSecurityPoliciesPaginatorName:
    return "list_security_policies"
```

```python
# ListSecurityPoliciesPaginatorName definition

ListSecurityPoliciesPaginatorName = Literal[
    "list_security_policies",
]
```
## ListServersPaginatorName

```python
# ListServersPaginatorName usage example

from types_aiobotocore_transfer.literals import ListServersPaginatorName

def get_value() -> ListServersPaginatorName:
    return "list_servers"
```

```python
# ListServersPaginatorName definition

ListServersPaginatorName = Literal[
    "list_servers",
]
```
## ListTagsForResourcePaginatorName

```python
# ListTagsForResourcePaginatorName usage example

from types_aiobotocore_transfer.literals import ListTagsForResourcePaginatorName

def get_value() -> ListTagsForResourcePaginatorName:
    return "list_tags_for_resource"
```

```python
# ListTagsForResourcePaginatorName definition

ListTagsForResourcePaginatorName = Literal[
    "list_tags_for_resource",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example

from types_aiobotocore_transfer.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition

ListUsersPaginatorName = Literal[
    "list_users",
]
```
## ListWorkflowsPaginatorName

```python
# ListWorkflowsPaginatorName usage example

from types_aiobotocore_transfer.literals import ListWorkflowsPaginatorName

def get_value() -> ListWorkflowsPaginatorName:
    return "list_workflows"
```

```python
# ListWorkflowsPaginatorName definition

ListWorkflowsPaginatorName = Literal[
    "list_workflows",
]
```
## MdnResponseType

```python
# MdnResponseType usage example

from types_aiobotocore_transfer.literals import MdnResponseType

def get_value() -> MdnResponseType:
    return "NONE"
```

```python
# MdnResponseType definition

MdnResponseType = Literal[
    "NONE",
    "SYNC",
]
```
## MdnSigningAlgType

```python
# MdnSigningAlgType usage example

from types_aiobotocore_transfer.literals import MdnSigningAlgType

def get_value() -> MdnSigningAlgType:
    return "DEFAULT"
```

```python
# MdnSigningAlgType definition

MdnSigningAlgType = Literal[
    "DEFAULT",
    "NONE",
    "SHA1",
    "SHA256",
    "SHA384",
    "SHA512",
]
```
## OverwriteExistingType

```python
# OverwriteExistingType usage example

from types_aiobotocore_transfer.literals import OverwriteExistingType

def get_value() -> OverwriteExistingType:
    return "FALSE"
```

```python
# OverwriteExistingType definition

OverwriteExistingType = Literal[
    "FALSE",
    "TRUE",
]
```
## ProfileTypeType

```python
# ProfileTypeType usage example

from types_aiobotocore_transfer.literals import ProfileTypeType

def get_value() -> ProfileTypeType:
    return "LOCAL"
```

```python
# ProfileTypeType definition

ProfileTypeType = Literal[
    "LOCAL",
    "PARTNER",
]
```
## ProtocolType

```python
# ProtocolType usage example

from types_aiobotocore_transfer.literals import ProtocolType

def get_value() -> ProtocolType:
    return "AS2"
```

```python
# ProtocolType definition

ProtocolType = Literal[
    "AS2",
    "FTP",
    "FTPS",
    "SFTP",
]
```
## ServerOfflineWaiterName

```python
# ServerOfflineWaiterName usage example

from types_aiobotocore_transfer.literals import ServerOfflineWaiterName

def get_value() -> ServerOfflineWaiterName:
    return "server_offline"
```

```python
# ServerOfflineWaiterName definition

ServerOfflineWaiterName = Literal[
    "server_offline",
]
```
## ServerOnlineWaiterName

```python
# ServerOnlineWaiterName usage example

from types_aiobotocore_transfer.literals import ServerOnlineWaiterName

def get_value() -> ServerOnlineWaiterName:
    return "server_online"
```

```python
# ServerOnlineWaiterName definition

ServerOnlineWaiterName = Literal[
    "server_online",
]
```
## SetStatOptionType

```python
# SetStatOptionType usage example

from types_aiobotocore_transfer.literals import SetStatOptionType

def get_value() -> SetStatOptionType:
    return "DEFAULT"
```

```python
# SetStatOptionType definition

SetStatOptionType = Literal[
    "DEFAULT",
    "ENABLE_NO_OP",
]
```
## SftpAuthenticationMethodsType

```python
# SftpAuthenticationMethodsType usage example

from types_aiobotocore_transfer.literals import SftpAuthenticationMethodsType

def get_value() -> SftpAuthenticationMethodsType:
    return "PASSWORD"
```

```python
# SftpAuthenticationMethodsType definition

SftpAuthenticationMethodsType = Literal[
    "PASSWORD",
    "PUBLIC_KEY",
    "PUBLIC_KEY_AND_PASSWORD",
    "PUBLIC_KEY_OR_PASSWORD",
]
```
## SigningAlgType

```python
# SigningAlgType usage example

from types_aiobotocore_transfer.literals import SigningAlgType

def get_value() -> SigningAlgType:
    return "NONE"
```

```python
# SigningAlgType definition

SigningAlgType = Literal[
    "NONE",
    "SHA1",
    "SHA256",
    "SHA384",
    "SHA512",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_transfer.literals import StateType

def get_value() -> StateType:
    return "OFFLINE"
```

```python
# StateType definition

StateType = Literal[
    "OFFLINE",
    "ONLINE",
    "START_FAILED",
    "STARTING",
    "STOP_FAILED",
    "STOPPING",
]
```
## TlsSessionResumptionModeType

```python
# TlsSessionResumptionModeType usage example

from types_aiobotocore_transfer.literals import TlsSessionResumptionModeType

def get_value() -> TlsSessionResumptionModeType:
    return "DISABLED"
```

```python
# TlsSessionResumptionModeType definition

TlsSessionResumptionModeType = Literal[
    "DISABLED",
    "ENABLED",
    "ENFORCED",
]
```
## WorkflowStepTypeType

```python
# WorkflowStepTypeType usage example

from types_aiobotocore_transfer.literals import WorkflowStepTypeType

def get_value() -> WorkflowStepTypeType:
    return "COPY"
```

```python
# WorkflowStepTypeType definition

WorkflowStepTypeType = Literal[
    "COPY",
    "CUSTOM",
    "DECRYPT",
    "DELETE",
    "TAG",
]
```
## TransferServiceName

```python
# TransferServiceName usage example

from types_aiobotocore_transfer.literals import TransferServiceName

def get_value() -> TransferServiceName:
    return "transfer"
```

```python
# TransferServiceName definition

TransferServiceName = Literal[
    "transfer",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_transfer.literals import ServiceName

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
    "alexaforbusiness",
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
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
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
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
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
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
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
    "fsx",
    "gamelift",
    "gamesparks",
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
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
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
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
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
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
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
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_transfer.literals import ResourceServiceName

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

from types_aiobotocore_transfer.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_accesses"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_accesses",
    "list_agreements",
    "list_certificates",
    "list_connectors",
    "list_executions",
    "list_profiles",
    "list_security_policies",
    "list_servers",
    "list_tags_for_resource",
    "list_users",
    "list_workflows",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_transfer.literals import WaiterName

def get_value() -> WaiterName:
    return "server_offline"
```

```python
# WaiterName definition

WaiterName = Literal[
    "server_offline",
    "server_online",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_transfer.literals import RegionName

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
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
