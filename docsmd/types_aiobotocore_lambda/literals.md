# Literals

> [Index](../README.md) > [Lambda](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## ApplicationLogLevelType

```python
# ApplicationLogLevelType usage example

from types_aiobotocore_lambda.literals import ApplicationLogLevelType

def get_value() -> ApplicationLogLevelType:
    return "DEBUG"
```

```python
# ApplicationLogLevelType definition

ApplicationLogLevelType = Literal[
    "DEBUG",
    "ERROR",
    "FATAL",
    "INFO",
    "TRACE",
    "WARN",
]
```
## ArchitectureType

```python
# ArchitectureType usage example

from types_aiobotocore_lambda.literals import ArchitectureType

def get_value() -> ArchitectureType:
    return "arm64"
```

```python
# ArchitectureType definition

ArchitectureType = Literal[
    "arm64",
    "x86_64",
]
```
## CodeSigningPolicyType

```python
# CodeSigningPolicyType usage example

from types_aiobotocore_lambda.literals import CodeSigningPolicyType

def get_value() -> CodeSigningPolicyType:
    return "Enforce"
```

```python
# CodeSigningPolicyType definition

CodeSigningPolicyType = Literal[
    "Enforce",
    "Warn",
]
```
## EndPointTypeType

```python
# EndPointTypeType usage example

from types_aiobotocore_lambda.literals import EndPointTypeType

def get_value() -> EndPointTypeType:
    return "KAFKA_BOOTSTRAP_SERVERS"
```

```python
# EndPointTypeType definition

EndPointTypeType = Literal[
    "KAFKA_BOOTSTRAP_SERVERS",
]
```
## EventSourceMappingMetricType

```python
# EventSourceMappingMetricType usage example

from types_aiobotocore_lambda.literals import EventSourceMappingMetricType

def get_value() -> EventSourceMappingMetricType:
    return "EventCount"
```

```python
# EventSourceMappingMetricType definition

EventSourceMappingMetricType = Literal[
    "EventCount",
]
```
## EventSourcePositionType

```python
# EventSourcePositionType usage example

from types_aiobotocore_lambda.literals import EventSourcePositionType

def get_value() -> EventSourcePositionType:
    return "AT_TIMESTAMP"
```

```python
# EventSourcePositionType definition

EventSourcePositionType = Literal[
    "AT_TIMESTAMP",
    "LATEST",
    "TRIM_HORIZON",
]
```
## FullDocumentType

```python
# FullDocumentType usage example

from types_aiobotocore_lambda.literals import FullDocumentType

def get_value() -> FullDocumentType:
    return "Default"
```

```python
# FullDocumentType definition

FullDocumentType = Literal[
    "Default",
    "UpdateLookup",
]
```
## FunctionActiveV2WaiterName

```python
# FunctionActiveV2WaiterName usage example

from types_aiobotocore_lambda.literals import FunctionActiveV2WaiterName

def get_value() -> FunctionActiveV2WaiterName:
    return "function_active_v2"
```

```python
# FunctionActiveV2WaiterName definition

FunctionActiveV2WaiterName = Literal[
    "function_active_v2",
]
```
## FunctionActiveWaiterName

```python
# FunctionActiveWaiterName usage example

from types_aiobotocore_lambda.literals import FunctionActiveWaiterName

def get_value() -> FunctionActiveWaiterName:
    return "function_active"
```

```python
# FunctionActiveWaiterName definition

FunctionActiveWaiterName = Literal[
    "function_active",
]
```
## FunctionExistsWaiterName

```python
# FunctionExistsWaiterName usage example

from types_aiobotocore_lambda.literals import FunctionExistsWaiterName

def get_value() -> FunctionExistsWaiterName:
    return "function_exists"
```

```python
# FunctionExistsWaiterName definition

FunctionExistsWaiterName = Literal[
    "function_exists",
]
```
## FunctionResponseTypeType

```python
# FunctionResponseTypeType usage example

from types_aiobotocore_lambda.literals import FunctionResponseTypeType

def get_value() -> FunctionResponseTypeType:
    return "ReportBatchItemFailures"
```

```python
# FunctionResponseTypeType definition

FunctionResponseTypeType = Literal[
    "ReportBatchItemFailures",
]
```
## FunctionUpdatedV2WaiterName

```python
# FunctionUpdatedV2WaiterName usage example

from types_aiobotocore_lambda.literals import FunctionUpdatedV2WaiterName

def get_value() -> FunctionUpdatedV2WaiterName:
    return "function_updated_v2"
```

```python
# FunctionUpdatedV2WaiterName definition

FunctionUpdatedV2WaiterName = Literal[
    "function_updated_v2",
]
```
## FunctionUpdatedWaiterName

```python
# FunctionUpdatedWaiterName usage example

from types_aiobotocore_lambda.literals import FunctionUpdatedWaiterName

def get_value() -> FunctionUpdatedWaiterName:
    return "function_updated"
```

```python
# FunctionUpdatedWaiterName definition

FunctionUpdatedWaiterName = Literal[
    "function_updated",
]
```
## FunctionUrlAuthTypeType

```python
# FunctionUrlAuthTypeType usage example

from types_aiobotocore_lambda.literals import FunctionUrlAuthTypeType

def get_value() -> FunctionUrlAuthTypeType:
    return "AWS_IAM"
```

```python
# FunctionUrlAuthTypeType definition

FunctionUrlAuthTypeType = Literal[
    "AWS_IAM",
    "NONE",
]
```
## FunctionVersionType

```python
# FunctionVersionType usage example

from types_aiobotocore_lambda.literals import FunctionVersionType

def get_value() -> FunctionVersionType:
    return "ALL"
```

```python
# FunctionVersionType definition

FunctionVersionType = Literal[
    "ALL",
]
```
## InvocationTypeType

```python
# InvocationTypeType usage example

from types_aiobotocore_lambda.literals import InvocationTypeType

def get_value() -> InvocationTypeType:
    return "DryRun"
```

```python
# InvocationTypeType definition

InvocationTypeType = Literal[
    "DryRun",
    "Event",
    "RequestResponse",
]
```
## InvokeModeType

```python
# InvokeModeType usage example

from types_aiobotocore_lambda.literals import InvokeModeType

def get_value() -> InvokeModeType:
    return "BUFFERED"
```

```python
# InvokeModeType definition

InvokeModeType = Literal[
    "BUFFERED",
    "RESPONSE_STREAM",
]
```
## LastUpdateStatusReasonCodeType

```python
# LastUpdateStatusReasonCodeType usage example

from types_aiobotocore_lambda.literals import LastUpdateStatusReasonCodeType

def get_value() -> LastUpdateStatusReasonCodeType:
    return "DisabledKMSKey"
```

```python
# LastUpdateStatusReasonCodeType definition

LastUpdateStatusReasonCodeType = Literal[
    "DisabledKMSKey",
    "EFSIOError",
    "EFSMountConnectivityError",
    "EFSMountFailure",
    "EFSMountTimeout",
    "EniLimitExceeded",
    "FunctionError",
    "ImageAccessDenied",
    "ImageDeleted",
    "InsufficientRolePermissions",
    "InternalError",
    "InvalidConfiguration",
    "InvalidImage",
    "InvalidRuntime",
    "InvalidSecurityGroup",
    "InvalidStateKMSKey",
    "InvalidSubnet",
    "InvalidZipFileException",
    "KMSKeyAccessDenied",
    "KMSKeyNotFound",
    "SubnetOutOfIPAddresses",
]
```
## LastUpdateStatusType

```python
# LastUpdateStatusType usage example

from types_aiobotocore_lambda.literals import LastUpdateStatusType

def get_value() -> LastUpdateStatusType:
    return "Failed"
```

```python
# LastUpdateStatusType definition

LastUpdateStatusType = Literal[
    "Failed",
    "InProgress",
    "Successful",
]
```
## ListAliasesPaginatorName

```python
# ListAliasesPaginatorName usage example

from types_aiobotocore_lambda.literals import ListAliasesPaginatorName

def get_value() -> ListAliasesPaginatorName:
    return "list_aliases"
```

```python
# ListAliasesPaginatorName definition

ListAliasesPaginatorName = Literal[
    "list_aliases",
]
```
## ListCodeSigningConfigsPaginatorName

```python
# ListCodeSigningConfigsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListCodeSigningConfigsPaginatorName

def get_value() -> ListCodeSigningConfigsPaginatorName:
    return "list_code_signing_configs"
```

```python
# ListCodeSigningConfigsPaginatorName definition

ListCodeSigningConfigsPaginatorName = Literal[
    "list_code_signing_configs",
]
```
## ListEventSourceMappingsPaginatorName

```python
# ListEventSourceMappingsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListEventSourceMappingsPaginatorName

def get_value() -> ListEventSourceMappingsPaginatorName:
    return "list_event_source_mappings"
```

```python
# ListEventSourceMappingsPaginatorName definition

ListEventSourceMappingsPaginatorName = Literal[
    "list_event_source_mappings",
]
```
## ListFunctionEventInvokeConfigsPaginatorName

```python
# ListFunctionEventInvokeConfigsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListFunctionEventInvokeConfigsPaginatorName

def get_value() -> ListFunctionEventInvokeConfigsPaginatorName:
    return "list_function_event_invoke_configs"
```

```python
# ListFunctionEventInvokeConfigsPaginatorName definition

ListFunctionEventInvokeConfigsPaginatorName = Literal[
    "list_function_event_invoke_configs",
]
```
## ListFunctionUrlConfigsPaginatorName

```python
# ListFunctionUrlConfigsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListFunctionUrlConfigsPaginatorName

def get_value() -> ListFunctionUrlConfigsPaginatorName:
    return "list_function_url_configs"
```

```python
# ListFunctionUrlConfigsPaginatorName definition

ListFunctionUrlConfigsPaginatorName = Literal[
    "list_function_url_configs",
]
```
## ListFunctionsByCodeSigningConfigPaginatorName

```python
# ListFunctionsByCodeSigningConfigPaginatorName usage example

from types_aiobotocore_lambda.literals import ListFunctionsByCodeSigningConfigPaginatorName

def get_value() -> ListFunctionsByCodeSigningConfigPaginatorName:
    return "list_functions_by_code_signing_config"
```

```python
# ListFunctionsByCodeSigningConfigPaginatorName definition

ListFunctionsByCodeSigningConfigPaginatorName = Literal[
    "list_functions_by_code_signing_config",
]
```
## ListFunctionsPaginatorName

```python
# ListFunctionsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListFunctionsPaginatorName

def get_value() -> ListFunctionsPaginatorName:
    return "list_functions"
```

```python
# ListFunctionsPaginatorName definition

ListFunctionsPaginatorName = Literal[
    "list_functions",
]
```
## ListLayerVersionsPaginatorName

```python
# ListLayerVersionsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListLayerVersionsPaginatorName

def get_value() -> ListLayerVersionsPaginatorName:
    return "list_layer_versions"
```

```python
# ListLayerVersionsPaginatorName definition

ListLayerVersionsPaginatorName = Literal[
    "list_layer_versions",
]
```
## ListLayersPaginatorName

```python
# ListLayersPaginatorName usage example

from types_aiobotocore_lambda.literals import ListLayersPaginatorName

def get_value() -> ListLayersPaginatorName:
    return "list_layers"
```

```python
# ListLayersPaginatorName definition

ListLayersPaginatorName = Literal[
    "list_layers",
]
```
## ListProvisionedConcurrencyConfigsPaginatorName

```python
# ListProvisionedConcurrencyConfigsPaginatorName usage example

from types_aiobotocore_lambda.literals import ListProvisionedConcurrencyConfigsPaginatorName

def get_value() -> ListProvisionedConcurrencyConfigsPaginatorName:
    return "list_provisioned_concurrency_configs"
```

```python
# ListProvisionedConcurrencyConfigsPaginatorName definition

ListProvisionedConcurrencyConfigsPaginatorName = Literal[
    "list_provisioned_concurrency_configs",
]
```
## ListVersionsByFunctionPaginatorName

```python
# ListVersionsByFunctionPaginatorName usage example

from types_aiobotocore_lambda.literals import ListVersionsByFunctionPaginatorName

def get_value() -> ListVersionsByFunctionPaginatorName:
    return "list_versions_by_function"
```

```python
# ListVersionsByFunctionPaginatorName definition

ListVersionsByFunctionPaginatorName = Literal[
    "list_versions_by_function",
]
```
## LogFormatType

```python
# LogFormatType usage example

from types_aiobotocore_lambda.literals import LogFormatType

def get_value() -> LogFormatType:
    return "JSON"
```

```python
# LogFormatType definition

LogFormatType = Literal[
    "JSON",
    "Text",
]
```
## LogTypeType

```python
# LogTypeType usage example

from types_aiobotocore_lambda.literals import LogTypeType

def get_value() -> LogTypeType:
    return "None"
```

```python
# LogTypeType definition

LogTypeType = Literal[
    "None",
    "Tail",
]
```
## PackageTypeType

```python
# PackageTypeType usage example

from types_aiobotocore_lambda.literals import PackageTypeType

def get_value() -> PackageTypeType:
    return "Image"
```

```python
# PackageTypeType definition

PackageTypeType = Literal[
    "Image",
    "Zip",
]
```
## ProvisionedConcurrencyStatusEnumType

```python
# ProvisionedConcurrencyStatusEnumType usage example

from types_aiobotocore_lambda.literals import ProvisionedConcurrencyStatusEnumType

def get_value() -> ProvisionedConcurrencyStatusEnumType:
    return "FAILED"
```

```python
# ProvisionedConcurrencyStatusEnumType definition

ProvisionedConcurrencyStatusEnumType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "READY",
]
```
## PublishedVersionActiveWaiterName

```python
# PublishedVersionActiveWaiterName usage example

from types_aiobotocore_lambda.literals import PublishedVersionActiveWaiterName

def get_value() -> PublishedVersionActiveWaiterName:
    return "published_version_active"
```

```python
# PublishedVersionActiveWaiterName definition

PublishedVersionActiveWaiterName = Literal[
    "published_version_active",
]
```
## RecursiveLoopType

```python
# RecursiveLoopType usage example

from types_aiobotocore_lambda.literals import RecursiveLoopType

def get_value() -> RecursiveLoopType:
    return "Allow"
```

```python
# RecursiveLoopType definition

RecursiveLoopType = Literal[
    "Allow",
    "Terminate",
]
```
## ResponseStreamingInvocationTypeType

```python
# ResponseStreamingInvocationTypeType usage example

from types_aiobotocore_lambda.literals import ResponseStreamingInvocationTypeType

def get_value() -> ResponseStreamingInvocationTypeType:
    return "DryRun"
```

```python
# ResponseStreamingInvocationTypeType definition

ResponseStreamingInvocationTypeType = Literal[
    "DryRun",
    "RequestResponse",
]
```
## RuntimeType

```python
# RuntimeType usage example

from types_aiobotocore_lambda.literals import RuntimeType

def get_value() -> RuntimeType:
    return "dotnet6"
```

```python
# RuntimeType definition

RuntimeType = Literal[
    "dotnet6",
    "dotnet8",
    "dotnetcore1.0",
    "dotnetcore2.0",
    "dotnetcore2.1",
    "dotnetcore3.1",
    "go1.x",
    "java11",
    "java17",
    "java21",
    "java8",
    "java8.al2",
    "nodejs",
    "nodejs10.x",
    "nodejs12.x",
    "nodejs14.x",
    "nodejs16.x",
    "nodejs18.x",
    "nodejs20.x",
    "nodejs22.x",
    "nodejs4.3",
    "nodejs4.3-edge",
    "nodejs6.10",
    "nodejs8.10",
    "provided",
    "provided.al2",
    "provided.al2023",
    "python2.7",
    "python3.10",
    "python3.11",
    "python3.12",
    "python3.13",
    "python3.6",
    "python3.7",
    "python3.8",
    "python3.9",
    "ruby2.5",
    "ruby2.7",
    "ruby3.2",
    "ruby3.3",
]
```
## SnapStartApplyOnType

```python
# SnapStartApplyOnType usage example

from types_aiobotocore_lambda.literals import SnapStartApplyOnType

def get_value() -> SnapStartApplyOnType:
    return "None"
```

```python
# SnapStartApplyOnType definition

SnapStartApplyOnType = Literal[
    "None",
    "PublishedVersions",
]
```
## SnapStartOptimizationStatusType

```python
# SnapStartOptimizationStatusType usage example

from types_aiobotocore_lambda.literals import SnapStartOptimizationStatusType

def get_value() -> SnapStartOptimizationStatusType:
    return "Off"
```

```python
# SnapStartOptimizationStatusType definition

SnapStartOptimizationStatusType = Literal[
    "Off",
    "On",
]
```
## SourceAccessTypeType

```python
# SourceAccessTypeType usage example

from types_aiobotocore_lambda.literals import SourceAccessTypeType

def get_value() -> SourceAccessTypeType:
    return "BASIC_AUTH"
```

```python
# SourceAccessTypeType definition

SourceAccessTypeType = Literal[
    "BASIC_AUTH",
    "CLIENT_CERTIFICATE_TLS_AUTH",
    "SASL_SCRAM_256_AUTH",
    "SASL_SCRAM_512_AUTH",
    "SERVER_ROOT_CA_CERTIFICATE",
    "VIRTUAL_HOST",
    "VPC_SECURITY_GROUP",
    "VPC_SUBNET",
]
```
## StateReasonCodeType

```python
# StateReasonCodeType usage example

from types_aiobotocore_lambda.literals import StateReasonCodeType

def get_value() -> StateReasonCodeType:
    return "Creating"
```

```python
# StateReasonCodeType definition

StateReasonCodeType = Literal[
    "Creating",
    "DisabledKMSKey",
    "EFSIOError",
    "EFSMountConnectivityError",
    "EFSMountFailure",
    "EFSMountTimeout",
    "EniLimitExceeded",
    "FunctionError",
    "Idle",
    "ImageAccessDenied",
    "ImageDeleted",
    "InsufficientRolePermissions",
    "InternalError",
    "InvalidConfiguration",
    "InvalidImage",
    "InvalidRuntime",
    "InvalidSecurityGroup",
    "InvalidStateKMSKey",
    "InvalidSubnet",
    "InvalidZipFileException",
    "KMSKeyAccessDenied",
    "KMSKeyNotFound",
    "Restoring",
    "SubnetOutOfIPAddresses",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_lambda.literals import StateType

def get_value() -> StateType:
    return "Active"
```

```python
# StateType definition

StateType = Literal[
    "Active",
    "Failed",
    "Inactive",
    "Pending",
]
```
## SystemLogLevelType

```python
# SystemLogLevelType usage example

from types_aiobotocore_lambda.literals import SystemLogLevelType

def get_value() -> SystemLogLevelType:
    return "DEBUG"
```

```python
# SystemLogLevelType definition

SystemLogLevelType = Literal[
    "DEBUG",
    "INFO",
    "WARN",
]
```
## TracingModeType

```python
# TracingModeType usage example

from types_aiobotocore_lambda.literals import TracingModeType

def get_value() -> TracingModeType:
    return "Active"
```

```python
# TracingModeType definition

TracingModeType = Literal[
    "Active",
    "PassThrough",
]
```
## UpdateRuntimeOnType

```python
# UpdateRuntimeOnType usage example

from types_aiobotocore_lambda.literals import UpdateRuntimeOnType

def get_value() -> UpdateRuntimeOnType:
    return "Auto"
```

```python
# UpdateRuntimeOnType definition

UpdateRuntimeOnType = Literal[
    "Auto",
    "FunctionUpdate",
    "Manual",
]
```
## LambdaServiceName

```python
# LambdaServiceName usage example

from types_aiobotocore_lambda.literals import LambdaServiceName

def get_value() -> LambdaServiceName:
    return "lambda"
```

```python
# LambdaServiceName definition

LambdaServiceName = Literal[
    "lambda",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_lambda.literals import ServiceName

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

from types_aiobotocore_lambda.literals import ResourceServiceName

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

from types_aiobotocore_lambda.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_aliases"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_aliases",
    "list_code_signing_configs",
    "list_event_source_mappings",
    "list_function_event_invoke_configs",
    "list_function_url_configs",
    "list_functions",
    "list_functions_by_code_signing_config",
    "list_layer_versions",
    "list_layers",
    "list_provisioned_concurrency_configs",
    "list_versions_by_function",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_lambda.literals import WaiterName

def get_value() -> WaiterName:
    return "function_active"
```

```python
# WaiterName definition

WaiterName = Literal[
    "function_active",
    "function_active_v2",
    "function_exists",
    "function_updated",
    "function_updated_v2",
    "published_version_active",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_lambda.literals import RegionName

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
