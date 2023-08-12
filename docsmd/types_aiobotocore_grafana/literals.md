# Literals

> [Index](../README.md) > [ManagedGrafana](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## AccountAccessTypeType

```python
# AccountAccessTypeType usage example

from types_aiobotocore_grafana.literals import AccountAccessTypeType

def get_value() -> AccountAccessTypeType:
    return "CURRENT_ACCOUNT"
```

```python
# AccountAccessTypeType definition

AccountAccessTypeType = Literal[
    "CURRENT_ACCOUNT",
    "ORGANIZATION",
]
```
## AuthenticationProviderTypesType

```python
# AuthenticationProviderTypesType usage example

from types_aiobotocore_grafana.literals import AuthenticationProviderTypesType

def get_value() -> AuthenticationProviderTypesType:
    return "AWS_SSO"
```

```python
# AuthenticationProviderTypesType definition

AuthenticationProviderTypesType = Literal[
    "AWS_SSO",
    "SAML",
]
```
## DataSourceTypeType

```python
# DataSourceTypeType usage example

from types_aiobotocore_grafana.literals import DataSourceTypeType

def get_value() -> DataSourceTypeType:
    return "AMAZON_OPENSEARCH_SERVICE"
```

```python
# DataSourceTypeType definition

DataSourceTypeType = Literal[
    "AMAZON_OPENSEARCH_SERVICE",
    "ATHENA",
    "CLOUDWATCH",
    "PROMETHEUS",
    "REDSHIFT",
    "SITEWISE",
    "TIMESTREAM",
    "TWINMAKER",
    "XRAY",
]
```
## LicenseTypeType

```python
# LicenseTypeType usage example

from types_aiobotocore_grafana.literals import LicenseTypeType

def get_value() -> LicenseTypeType:
    return "ENTERPRISE"
```

```python
# LicenseTypeType definition

LicenseTypeType = Literal[
    "ENTERPRISE",
    "ENTERPRISE_FREE_TRIAL",
]
```
## ListPermissionsPaginatorName

```python
# ListPermissionsPaginatorName usage example

from types_aiobotocore_grafana.literals import ListPermissionsPaginatorName

def get_value() -> ListPermissionsPaginatorName:
    return "list_permissions"
```

```python
# ListPermissionsPaginatorName definition

ListPermissionsPaginatorName = Literal[
    "list_permissions",
]
```
## ListVersionsPaginatorName

```python
# ListVersionsPaginatorName usage example

from types_aiobotocore_grafana.literals import ListVersionsPaginatorName

def get_value() -> ListVersionsPaginatorName:
    return "list_versions"
```

```python
# ListVersionsPaginatorName definition

ListVersionsPaginatorName = Literal[
    "list_versions",
]
```
## ListWorkspacesPaginatorName

```python
# ListWorkspacesPaginatorName usage example

from types_aiobotocore_grafana.literals import ListWorkspacesPaginatorName

def get_value() -> ListWorkspacesPaginatorName:
    return "list_workspaces"
```

```python
# ListWorkspacesPaginatorName definition

ListWorkspacesPaginatorName = Literal[
    "list_workspaces",
]
```
## NotificationDestinationTypeType

```python
# NotificationDestinationTypeType usage example

from types_aiobotocore_grafana.literals import NotificationDestinationTypeType

def get_value() -> NotificationDestinationTypeType:
    return "SNS"
```

```python
# NotificationDestinationTypeType definition

NotificationDestinationTypeType = Literal[
    "SNS",
]
```
## PermissionTypeType

```python
# PermissionTypeType usage example

from types_aiobotocore_grafana.literals import PermissionTypeType

def get_value() -> PermissionTypeType:
    return "CUSTOMER_MANAGED"
```

```python
# PermissionTypeType definition

PermissionTypeType = Literal[
    "CUSTOMER_MANAGED",
    "SERVICE_MANAGED",
]
```
## RoleType

```python
# RoleType usage example

from types_aiobotocore_grafana.literals import RoleType

def get_value() -> RoleType:
    return "ADMIN"
```

```python
# RoleType definition

RoleType = Literal[
    "ADMIN",
    "EDITOR",
    "VIEWER",
]
```
## SamlConfigurationStatusType

```python
# SamlConfigurationStatusType usage example

from types_aiobotocore_grafana.literals import SamlConfigurationStatusType

def get_value() -> SamlConfigurationStatusType:
    return "CONFIGURED"
```

```python
# SamlConfigurationStatusType definition

SamlConfigurationStatusType = Literal[
    "CONFIGURED",
    "NOT_CONFIGURED",
]
```
## UpdateActionType

```python
# UpdateActionType usage example

from types_aiobotocore_grafana.literals import UpdateActionType

def get_value() -> UpdateActionType:
    return "ADD"
```

```python
# UpdateActionType definition

UpdateActionType = Literal[
    "ADD",
    "REVOKE",
]
```
## UserTypeType

```python
# UserTypeType usage example

from types_aiobotocore_grafana.literals import UserTypeType

def get_value() -> UserTypeType:
    return "SSO_GROUP"
```

```python
# UserTypeType definition

UserTypeType = Literal[
    "SSO_GROUP",
    "SSO_USER",
]
```
## WorkspaceStatusType

```python
# WorkspaceStatusType usage example

from types_aiobotocore_grafana.literals import WorkspaceStatusType

def get_value() -> WorkspaceStatusType:
    return "ACTIVE"
```

```python
# WorkspaceStatusType definition

WorkspaceStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "CREATION_FAILED",
    "DELETING",
    "DELETION_FAILED",
    "FAILED",
    "LICENSE_REMOVAL_FAILED",
    "UPDATE_FAILED",
    "UPDATING",
    "UPGRADE_FAILED",
    "UPGRADING",
    "VERSION_UPDATE_FAILED",
    "VERSION_UPDATING",
]
```
## ManagedGrafanaServiceName

```python
# ManagedGrafanaServiceName usage example

from types_aiobotocore_grafana.literals import ManagedGrafanaServiceName

def get_value() -> ManagedGrafanaServiceName:
    return "grafana"
```

```python
# ManagedGrafanaServiceName definition

ManagedGrafanaServiceName = Literal[
    "grafana",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_grafana.literals import ServiceName

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

from types_aiobotocore_grafana.literals import ResourceServiceName

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

from types_aiobotocore_grafana.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_permissions"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_permissions",
    "list_versions",
    "list_workspaces",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_grafana.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
