# Literals

> [Index](../README.md) > [BedrockAgentCore](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## AutomationStreamStatusType

```python
# AutomationStreamStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import AutomationStreamStatusType

def get_value() -> AutomationStreamStatusType:
    return "DISABLED"
```

```python
# AutomationStreamStatusType definition
AutomationStreamStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## BrowserSessionStatusType

```python
# BrowserSessionStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import BrowserSessionStatusType

def get_value() -> BrowserSessionStatusType:
    return "READY"
```

```python
# BrowserSessionStatusType definition
BrowserSessionStatusType = Literal[
    "READY",
    "TERMINATED",
]
```
## CodeInterpreterSessionStatusType

```python
# CodeInterpreterSessionStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import CodeInterpreterSessionStatusType

def get_value() -> CodeInterpreterSessionStatusType:
    return "READY"
```

```python
# CodeInterpreterSessionStatusType definition
CodeInterpreterSessionStatusType = Literal[
    "READY",
    "TERMINATED",
]
```
## ContentBlockTypeType

```python
# ContentBlockTypeType usage example
from types_aiobotocore_bedrock_agentcore.literals import ContentBlockTypeType

def get_value() -> ContentBlockTypeType:
    return "image"
```

```python
# ContentBlockTypeType definition
ContentBlockTypeType = Literal[
    "image",
    "resource",
    "resource_link",
    "text",
]
```
## ExtractionJobStatusType

```python
# ExtractionJobStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import ExtractionJobStatusType

def get_value() -> ExtractionJobStatusType:
    return "FAILED"
```

```python
# ExtractionJobStatusType definition
ExtractionJobStatusType = Literal[
    "FAILED",
]
```
## ListActorsPaginatorName

```python
# ListActorsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import ListActorsPaginatorName

def get_value() -> ListActorsPaginatorName:
    return "list_actors"
```

```python
# ListActorsPaginatorName definition
ListActorsPaginatorName = Literal[
    "list_actors",
]
```
## ListEventsPaginatorName

```python
# ListEventsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import ListEventsPaginatorName

def get_value() -> ListEventsPaginatorName:
    return "list_events"
```

```python
# ListEventsPaginatorName definition
ListEventsPaginatorName = Literal[
    "list_events",
]
```
## ListMemoryExtractionJobsPaginatorName

```python
# ListMemoryExtractionJobsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import ListMemoryExtractionJobsPaginatorName

def get_value() -> ListMemoryExtractionJobsPaginatorName:
    return "list_memory_extraction_jobs"
```

```python
# ListMemoryExtractionJobsPaginatorName definition
ListMemoryExtractionJobsPaginatorName = Literal[
    "list_memory_extraction_jobs",
]
```
## ListMemoryRecordsPaginatorName

```python
# ListMemoryRecordsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import ListMemoryRecordsPaginatorName

def get_value() -> ListMemoryRecordsPaginatorName:
    return "list_memory_records"
```

```python
# ListMemoryRecordsPaginatorName definition
ListMemoryRecordsPaginatorName = Literal[
    "list_memory_records",
]
```
## ListSessionsPaginatorName

```python
# ListSessionsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import ListSessionsPaginatorName

def get_value() -> ListSessionsPaginatorName:
    return "list_sessions"
```

```python
# ListSessionsPaginatorName definition
ListSessionsPaginatorName = Literal[
    "list_sessions",
]
```
## MemoryRecordStatusType

```python
# MemoryRecordStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import MemoryRecordStatusType

def get_value() -> MemoryRecordStatusType:
    return "FAILED"
```

```python
# MemoryRecordStatusType definition
MemoryRecordStatusType = Literal[
    "FAILED",
    "SUCCEEDED",
]
```
## Oauth2FlowTypeType

```python
# Oauth2FlowTypeType usage example
from types_aiobotocore_bedrock_agentcore.literals import Oauth2FlowTypeType

def get_value() -> Oauth2FlowTypeType:
    return "M2M"
```

```python
# Oauth2FlowTypeType definition
Oauth2FlowTypeType = Literal[
    "M2M",
    "USER_FEDERATION",
]
```
## OperatorTypeType

```python
# OperatorTypeType usage example
from types_aiobotocore_bedrock_agentcore.literals import OperatorTypeType

def get_value() -> OperatorTypeType:
    return "EQUALS_TO"
```

```python
# OperatorTypeType definition
OperatorTypeType = Literal[
    "EQUALS_TO",
    "EXISTS",
    "NOT_EXISTS",
]
```
## ProgrammingLanguageType

```python
# ProgrammingLanguageType usage example
from types_aiobotocore_bedrock_agentcore.literals import ProgrammingLanguageType

def get_value() -> ProgrammingLanguageType:
    return "javascript"
```

```python
# ProgrammingLanguageType definition
ProgrammingLanguageType = Literal[
    "javascript",
    "python",
    "typescript",
]
```
## ResourceContentTypeType

```python
# ResourceContentTypeType usage example
from types_aiobotocore_bedrock_agentcore.literals import ResourceContentTypeType

def get_value() -> ResourceContentTypeType:
    return "blob"
```

```python
# ResourceContentTypeType definition
ResourceContentTypeType = Literal[
    "blob",
    "text",
]
```
## RetrieveMemoryRecordsPaginatorName

```python
# RetrieveMemoryRecordsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore.literals import RetrieveMemoryRecordsPaginatorName

def get_value() -> RetrieveMemoryRecordsPaginatorName:
    return "retrieve_memory_records"
```

```python
# RetrieveMemoryRecordsPaginatorName definition
RetrieveMemoryRecordsPaginatorName = Literal[
    "retrieve_memory_records",
]
```
## RoleType

```python
# RoleType usage example
from types_aiobotocore_bedrock_agentcore.literals import RoleType

def get_value() -> RoleType:
    return "ASSISTANT"
```

```python
# RoleType definition
RoleType = Literal[
    "ASSISTANT",
    "OTHER",
    "TOOL",
    "USER",
]
```
## SessionStatusType

```python
# SessionStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import SessionStatusType

def get_value() -> SessionStatusType:
    return "FAILED"
```

```python
# SessionStatusType definition
SessionStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
]
```
## TaskStatusType

```python
# TaskStatusType usage example
from types_aiobotocore_bedrock_agentcore.literals import TaskStatusType

def get_value() -> TaskStatusType:
    return "canceled"
```

```python
# TaskStatusType definition
TaskStatusType = Literal[
    "canceled",
    "completed",
    "failed",
    "submitted",
    "working",
]
```
## ToolNameType

```python
# ToolNameType usage example
from types_aiobotocore_bedrock_agentcore.literals import ToolNameType

def get_value() -> ToolNameType:
    return "executeCode"
```

```python
# ToolNameType definition
ToolNameType = Literal[
    "executeCode",
    "executeCommand",
    "getTask",
    "listFiles",
    "readFiles",
    "removeFiles",
    "startCommandExecution",
    "stopTask",
    "writeFiles",
]
```
## ValidationExceptionReasonType

```python
# ValidationExceptionReasonType usage example
from types_aiobotocore_bedrock_agentcore.literals import ValidationExceptionReasonType

def get_value() -> ValidationExceptionReasonType:
    return "CannotParse"
```

```python
# ValidationExceptionReasonType definition
ValidationExceptionReasonType = Literal[
    "CannotParse",
    "EventInOtherSession",
    "FieldValidationFailed",
    "IdempotentParameterMismatchException",
    "ResourceConflict",
]
```
## BedrockAgentCoreServiceName

```python
# BedrockAgentCoreServiceName usage example
from types_aiobotocore_bedrock_agentcore.literals import BedrockAgentCoreServiceName

def get_value() -> BedrockAgentCoreServiceName:
    return "bedrock-agentcore"
```

```python
# BedrockAgentCoreServiceName definition
BedrockAgentCoreServiceName = Literal[
    "bedrock-agentcore",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_bedrock_agentcore.literals import ServiceName

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
from types_aiobotocore_bedrock_agentcore.literals import ResourceServiceName

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
from types_aiobotocore_bedrock_agentcore.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_actors"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_actors",
    "list_events",
    "list_memory_extraction_jobs",
    "list_memory_records",
    "list_sessions",
    "retrieve_memory_records",
]
```
