# Literals

> [Index](../README.md) > [CodeCatalyst](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## ComparisonOperatorType

```python
# ComparisonOperatorType usage example

from types_aiobotocore_codecatalyst.literals import ComparisonOperatorType

def get_value() -> ComparisonOperatorType:
    return "EQ"
```

```python
# ComparisonOperatorType definition

ComparisonOperatorType = Literal[
    "EQ",
    "GE",
    "GT",
    "LE",
    "LT",
]
```
## DevEnvironmentSessionTypeType

```python
# DevEnvironmentSessionTypeType usage example

from types_aiobotocore_codecatalyst.literals import DevEnvironmentSessionTypeType

def get_value() -> DevEnvironmentSessionTypeType:
    return "SSH"
```

```python
# DevEnvironmentSessionTypeType definition

DevEnvironmentSessionTypeType = Literal[
    "SSH",
    "SSM",
]
```
## DevEnvironmentStatusType

```python
# DevEnvironmentStatusType usage example

from types_aiobotocore_codecatalyst.literals import DevEnvironmentStatusType

def get_value() -> DevEnvironmentStatusType:
    return "DELETED"
```

```python
# DevEnvironmentStatusType definition

DevEnvironmentStatusType = Literal[
    "DELETED",
    "DELETING",
    "FAILED",
    "PENDING",
    "RUNNING",
    "STARTING",
    "STOPPED",
    "STOPPING",
]
```
## FilterKeyType

```python
# FilterKeyType usage example

from types_aiobotocore_codecatalyst.literals import FilterKeyType

def get_value() -> FilterKeyType:
    return "hasAccessTo"
```

```python
# FilterKeyType definition

FilterKeyType = Literal[
    "hasAccessTo",
]
```
## InstanceTypeType

```python
# InstanceTypeType usage example

from types_aiobotocore_codecatalyst.literals import InstanceTypeType

def get_value() -> InstanceTypeType:
    return "dev.standard1.large"
```

```python
# InstanceTypeType definition

InstanceTypeType = Literal[
    "dev.standard1.large",
    "dev.standard1.medium",
    "dev.standard1.small",
    "dev.standard1.xlarge",
]
```
## ListAccessTokensPaginatorName

```python
# ListAccessTokensPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListAccessTokensPaginatorName

def get_value() -> ListAccessTokensPaginatorName:
    return "list_access_tokens"
```

```python
# ListAccessTokensPaginatorName definition

ListAccessTokensPaginatorName = Literal[
    "list_access_tokens",
]
```
## ListDevEnvironmentSessionsPaginatorName

```python
# ListDevEnvironmentSessionsPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListDevEnvironmentSessionsPaginatorName

def get_value() -> ListDevEnvironmentSessionsPaginatorName:
    return "list_dev_environment_sessions"
```

```python
# ListDevEnvironmentSessionsPaginatorName definition

ListDevEnvironmentSessionsPaginatorName = Literal[
    "list_dev_environment_sessions",
]
```
## ListDevEnvironmentsPaginatorName

```python
# ListDevEnvironmentsPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListDevEnvironmentsPaginatorName

def get_value() -> ListDevEnvironmentsPaginatorName:
    return "list_dev_environments"
```

```python
# ListDevEnvironmentsPaginatorName definition

ListDevEnvironmentsPaginatorName = Literal[
    "list_dev_environments",
]
```
## ListEventLogsPaginatorName

```python
# ListEventLogsPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListEventLogsPaginatorName

def get_value() -> ListEventLogsPaginatorName:
    return "list_event_logs"
```

```python
# ListEventLogsPaginatorName definition

ListEventLogsPaginatorName = Literal[
    "list_event_logs",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition

ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ListSourceRepositoriesPaginatorName

```python
# ListSourceRepositoriesPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListSourceRepositoriesPaginatorName

def get_value() -> ListSourceRepositoriesPaginatorName:
    return "list_source_repositories"
```

```python
# ListSourceRepositoriesPaginatorName definition

ListSourceRepositoriesPaginatorName = Literal[
    "list_source_repositories",
]
```
## ListSourceRepositoryBranchesPaginatorName

```python
# ListSourceRepositoryBranchesPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListSourceRepositoryBranchesPaginatorName

def get_value() -> ListSourceRepositoryBranchesPaginatorName:
    return "list_source_repository_branches"
```

```python
# ListSourceRepositoryBranchesPaginatorName definition

ListSourceRepositoryBranchesPaginatorName = Literal[
    "list_source_repository_branches",
]
```
## ListSpacesPaginatorName

```python
# ListSpacesPaginatorName usage example

from types_aiobotocore_codecatalyst.literals import ListSpacesPaginatorName

def get_value() -> ListSpacesPaginatorName:
    return "list_spaces"
```

```python
# ListSpacesPaginatorName definition

ListSpacesPaginatorName = Literal[
    "list_spaces",
]
```
## OperationTypeType

```python
# OperationTypeType usage example

from types_aiobotocore_codecatalyst.literals import OperationTypeType

def get_value() -> OperationTypeType:
    return "MUTATION"
```

```python
# OperationTypeType definition

OperationTypeType = Literal[
    "MUTATION",
    "READONLY",
]
```
## UserTypeType

```python
# UserTypeType usage example

from types_aiobotocore_codecatalyst.literals import UserTypeType

def get_value() -> UserTypeType:
    return "AWS_ACCOUNT"
```

```python
# UserTypeType definition

UserTypeType = Literal[
    "AWS_ACCOUNT",
    "UNKNOWN",
    "USER",
]
```
## CodeCatalystServiceName

```python
# CodeCatalystServiceName usage example

from types_aiobotocore_codecatalyst.literals import CodeCatalystServiceName

def get_value() -> CodeCatalystServiceName:
    return "codecatalyst"
```

```python
# CodeCatalystServiceName definition

CodeCatalystServiceName = Literal[
    "codecatalyst",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_codecatalyst.literals import ServiceName

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

from types_aiobotocore_codecatalyst.literals import ResourceServiceName

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

from types_aiobotocore_codecatalyst.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_access_tokens"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_access_tokens",
    "list_dev_environment_sessions",
    "list_dev_environments",
    "list_event_logs",
    "list_projects",
    "list_source_repositories",
    "list_source_repository_branches",
    "list_spaces",
]
```
