# Literals

> [Index](../README.md) > [AppSync](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## ApiCacheStatusType

```python
# ApiCacheStatusType usage example

from types_aiobotocore_appsync.literals import ApiCacheStatusType

def get_value() -> ApiCacheStatusType:
    return "AVAILABLE"
```

```python
# ApiCacheStatusType definition

ApiCacheStatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "FAILED",
    "MODIFYING",
]
```
## ApiCacheTypeType

```python
# ApiCacheTypeType usage example

from types_aiobotocore_appsync.literals import ApiCacheTypeType

def get_value() -> ApiCacheTypeType:
    return "LARGE"
```

```python
# ApiCacheTypeType definition

ApiCacheTypeType = Literal[
    "LARGE",
    "LARGE_12X",
    "LARGE_2X",
    "LARGE_4X",
    "LARGE_8X",
    "MEDIUM",
    "R4_2XLARGE",
    "R4_4XLARGE",
    "R4_8XLARGE",
    "R4_LARGE",
    "R4_XLARGE",
    "SMALL",
    "T2_MEDIUM",
    "T2_SMALL",
    "XLARGE",
]
```
## ApiCachingBehaviorType

```python
# ApiCachingBehaviorType usage example

from types_aiobotocore_appsync.literals import ApiCachingBehaviorType

def get_value() -> ApiCachingBehaviorType:
    return "FULL_REQUEST_CACHING"
```

```python
# ApiCachingBehaviorType definition

ApiCachingBehaviorType = Literal[
    "FULL_REQUEST_CACHING",
    "PER_RESOLVER_CACHING",
]
```
## AssociationStatusType

```python
# AssociationStatusType usage example

from types_aiobotocore_appsync.literals import AssociationStatusType

def get_value() -> AssociationStatusType:
    return "FAILED"
```

```python
# AssociationStatusType definition

AssociationStatusType = Literal[
    "FAILED",
    "PROCESSING",
    "SUCCESS",
]
```
## AuthenticationTypeType

```python
# AuthenticationTypeType usage example

from types_aiobotocore_appsync.literals import AuthenticationTypeType

def get_value() -> AuthenticationTypeType:
    return "AMAZON_COGNITO_USER_POOLS"
```

```python
# AuthenticationTypeType definition

AuthenticationTypeType = Literal[
    "AMAZON_COGNITO_USER_POOLS",
    "API_KEY",
    "AWS_IAM",
    "AWS_LAMBDA",
    "OPENID_CONNECT",
]
```
## AuthorizationTypeType

```python
# AuthorizationTypeType usage example

from types_aiobotocore_appsync.literals import AuthorizationTypeType

def get_value() -> AuthorizationTypeType:
    return "AWS_IAM"
```

```python
# AuthorizationTypeType definition

AuthorizationTypeType = Literal[
    "AWS_IAM",
]
```
## ConflictDetectionTypeType

```python
# ConflictDetectionTypeType usage example

from types_aiobotocore_appsync.literals import ConflictDetectionTypeType

def get_value() -> ConflictDetectionTypeType:
    return "NONE"
```

```python
# ConflictDetectionTypeType definition

ConflictDetectionTypeType = Literal[
    "NONE",
    "VERSION",
]
```
## ConflictHandlerTypeType

```python
# ConflictHandlerTypeType usage example

from types_aiobotocore_appsync.literals import ConflictHandlerTypeType

def get_value() -> ConflictHandlerTypeType:
    return "AUTOMERGE"
```

```python
# ConflictHandlerTypeType definition

ConflictHandlerTypeType = Literal[
    "AUTOMERGE",
    "LAMBDA",
    "NONE",
    "OPTIMISTIC_CONCURRENCY",
]
```
## DataSourceTypeType

```python
# DataSourceTypeType usage example

from types_aiobotocore_appsync.literals import DataSourceTypeType

def get_value() -> DataSourceTypeType:
    return "AMAZON_DYNAMODB"
```

```python
# DataSourceTypeType definition

DataSourceTypeType = Literal[
    "AMAZON_DYNAMODB",
    "AMAZON_ELASTICSEARCH",
    "AMAZON_EVENTBRIDGE",
    "AMAZON_OPENSEARCH_SERVICE",
    "AWS_LAMBDA",
    "HTTP",
    "NONE",
    "RELATIONAL_DATABASE",
]
```
## DefaultActionType

```python
# DefaultActionType usage example

from types_aiobotocore_appsync.literals import DefaultActionType

def get_value() -> DefaultActionType:
    return "ALLOW"
```

```python
# DefaultActionType definition

DefaultActionType = Literal[
    "ALLOW",
    "DENY",
]
```
## FieldLogLevelType

```python
# FieldLogLevelType usage example

from types_aiobotocore_appsync.literals import FieldLogLevelType

def get_value() -> FieldLogLevelType:
    return "ALL"
```

```python
# FieldLogLevelType definition

FieldLogLevelType = Literal[
    "ALL",
    "ERROR",
    "NONE",
]
```
## GraphQLApiTypeType

```python
# GraphQLApiTypeType usage example

from types_aiobotocore_appsync.literals import GraphQLApiTypeType

def get_value() -> GraphQLApiTypeType:
    return "GRAPHQL"
```

```python
# GraphQLApiTypeType definition

GraphQLApiTypeType = Literal[
    "GRAPHQL",
    "MERGED",
]
```
## GraphQLApiVisibilityType

```python
# GraphQLApiVisibilityType usage example

from types_aiobotocore_appsync.literals import GraphQLApiVisibilityType

def get_value() -> GraphQLApiVisibilityType:
    return "GLOBAL"
```

```python
# GraphQLApiVisibilityType definition

GraphQLApiVisibilityType = Literal[
    "GLOBAL",
    "PRIVATE",
]
```
## ListApiKeysPaginatorName

```python
# ListApiKeysPaginatorName usage example

from types_aiobotocore_appsync.literals import ListApiKeysPaginatorName

def get_value() -> ListApiKeysPaginatorName:
    return "list_api_keys"
```

```python
# ListApiKeysPaginatorName definition

ListApiKeysPaginatorName = Literal[
    "list_api_keys",
]
```
## ListDataSourcesPaginatorName

```python
# ListDataSourcesPaginatorName usage example

from types_aiobotocore_appsync.literals import ListDataSourcesPaginatorName

def get_value() -> ListDataSourcesPaginatorName:
    return "list_data_sources"
```

```python
# ListDataSourcesPaginatorName definition

ListDataSourcesPaginatorName = Literal[
    "list_data_sources",
]
```
## ListFunctionsPaginatorName

```python
# ListFunctionsPaginatorName usage example

from types_aiobotocore_appsync.literals import ListFunctionsPaginatorName

def get_value() -> ListFunctionsPaginatorName:
    return "list_functions"
```

```python
# ListFunctionsPaginatorName definition

ListFunctionsPaginatorName = Literal[
    "list_functions",
]
```
## ListGraphqlApisPaginatorName

```python
# ListGraphqlApisPaginatorName usage example

from types_aiobotocore_appsync.literals import ListGraphqlApisPaginatorName

def get_value() -> ListGraphqlApisPaginatorName:
    return "list_graphql_apis"
```

```python
# ListGraphqlApisPaginatorName definition

ListGraphqlApisPaginatorName = Literal[
    "list_graphql_apis",
]
```
## ListResolversByFunctionPaginatorName

```python
# ListResolversByFunctionPaginatorName usage example

from types_aiobotocore_appsync.literals import ListResolversByFunctionPaginatorName

def get_value() -> ListResolversByFunctionPaginatorName:
    return "list_resolvers_by_function"
```

```python
# ListResolversByFunctionPaginatorName definition

ListResolversByFunctionPaginatorName = Literal[
    "list_resolvers_by_function",
]
```
## ListResolversPaginatorName

```python
# ListResolversPaginatorName usage example

from types_aiobotocore_appsync.literals import ListResolversPaginatorName

def get_value() -> ListResolversPaginatorName:
    return "list_resolvers"
```

```python
# ListResolversPaginatorName definition

ListResolversPaginatorName = Literal[
    "list_resolvers",
]
```
## ListTypesPaginatorName

```python
# ListTypesPaginatorName usage example

from types_aiobotocore_appsync.literals import ListTypesPaginatorName

def get_value() -> ListTypesPaginatorName:
    return "list_types"
```

```python
# ListTypesPaginatorName definition

ListTypesPaginatorName = Literal[
    "list_types",
]
```
## MergeTypeType

```python
# MergeTypeType usage example

from types_aiobotocore_appsync.literals import MergeTypeType

def get_value() -> MergeTypeType:
    return "AUTO_MERGE"
```

```python
# MergeTypeType definition

MergeTypeType = Literal[
    "AUTO_MERGE",
    "MANUAL_MERGE",
]
```
## OutputTypeType

```python
# OutputTypeType usage example

from types_aiobotocore_appsync.literals import OutputTypeType

def get_value() -> OutputTypeType:
    return "JSON"
```

```python
# OutputTypeType definition

OutputTypeType = Literal[
    "JSON",
    "SDL",
]
```
## OwnershipType

```python
# OwnershipType usage example

from types_aiobotocore_appsync.literals import OwnershipType

def get_value() -> OwnershipType:
    return "CURRENT_ACCOUNT"
```

```python
# OwnershipType definition

OwnershipType = Literal[
    "CURRENT_ACCOUNT",
    "OTHER_ACCOUNTS",
]
```
## RelationalDatabaseSourceTypeType

```python
# RelationalDatabaseSourceTypeType usage example

from types_aiobotocore_appsync.literals import RelationalDatabaseSourceTypeType

def get_value() -> RelationalDatabaseSourceTypeType:
    return "RDS_HTTP_ENDPOINT"
```

```python
# RelationalDatabaseSourceTypeType definition

RelationalDatabaseSourceTypeType = Literal[
    "RDS_HTTP_ENDPOINT",
]
```
## ResolverKindType

```python
# ResolverKindType usage example

from types_aiobotocore_appsync.literals import ResolverKindType

def get_value() -> ResolverKindType:
    return "PIPELINE"
```

```python
# ResolverKindType definition

ResolverKindType = Literal[
    "PIPELINE",
    "UNIT",
]
```
## RuntimeNameType

```python
# RuntimeNameType usage example

from types_aiobotocore_appsync.literals import RuntimeNameType

def get_value() -> RuntimeNameType:
    return "APPSYNC_JS"
```

```python
# RuntimeNameType definition

RuntimeNameType = Literal[
    "APPSYNC_JS",
]
```
## SchemaStatusType

```python
# SchemaStatusType usage example

from types_aiobotocore_appsync.literals import SchemaStatusType

def get_value() -> SchemaStatusType:
    return "ACTIVE"
```

```python
# SchemaStatusType definition

SchemaStatusType = Literal[
    "ACTIVE",
    "DELETING",
    "FAILED",
    "NOT_APPLICABLE",
    "PROCESSING",
    "SUCCESS",
]
```
## SourceApiAssociationStatusType

```python
# SourceApiAssociationStatusType usage example

from types_aiobotocore_appsync.literals import SourceApiAssociationStatusType

def get_value() -> SourceApiAssociationStatusType:
    return "AUTO_MERGE_SCHEDULE_FAILED"
```

```python
# SourceApiAssociationStatusType definition

SourceApiAssociationStatusType = Literal[
    "AUTO_MERGE_SCHEDULE_FAILED",
    "DELETION_FAILED",
    "DELETION_IN_PROGRESS",
    "DELETION_SCHEDULED",
    "MERGE_FAILED",
    "MERGE_IN_PROGRESS",
    "MERGE_SCHEDULED",
    "MERGE_SUCCESS",
]
```
## TypeDefinitionFormatType

```python
# TypeDefinitionFormatType usage example

from types_aiobotocore_appsync.literals import TypeDefinitionFormatType

def get_value() -> TypeDefinitionFormatType:
    return "JSON"
```

```python
# TypeDefinitionFormatType definition

TypeDefinitionFormatType = Literal[
    "JSON",
    "SDL",
]
```
## AppSyncServiceName

```python
# AppSyncServiceName usage example

from types_aiobotocore_appsync.literals import AppSyncServiceName

def get_value() -> AppSyncServiceName:
    return "appsync"
```

```python
# AppSyncServiceName definition

AppSyncServiceName = Literal[
    "appsync",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_appsync.literals import ServiceName

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

from types_aiobotocore_appsync.literals import ResourceServiceName

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

from types_aiobotocore_appsync.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_api_keys"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_api_keys",
    "list_data_sources",
    "list_functions",
    "list_graphql_apis",
    "list_resolvers",
    "list_resolvers_by_function",
    "list_types",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_appsync.literals import RegionName

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
