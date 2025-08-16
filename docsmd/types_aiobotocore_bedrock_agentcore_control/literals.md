# Literals

> [Index](../README.md) > [BedrockAgentCoreControlPlaneFrontingLayer](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControlPlaneFrontingLayer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrolplanefrontinglayer)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## AgentEndpointStatusType

```python
# AgentEndpointStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AgentEndpointStatusType

def get_value() -> AgentEndpointStatusType:
    return "CREATE_FAILED"
```

```python
# AgentEndpointStatusType definition
AgentEndpointStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "READY",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## AgentStatusType

```python
# AgentStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AgentStatusType

def get_value() -> AgentStatusType:
    return "CREATE_FAILED"
```

```python
# AgentStatusType definition
AgentStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "READY",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ApiKeyCredentialLocationType

```python
# ApiKeyCredentialLocationType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ApiKeyCredentialLocationType

def get_value() -> ApiKeyCredentialLocationType:
    return "HEADER"
```

```python
# ApiKeyCredentialLocationType definition
ApiKeyCredentialLocationType = Literal[
    "HEADER",
    "QUERY_PARAMETER",
]
```
## AuthorizerTypeType

```python
# AuthorizerTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AuthorizerTypeType

def get_value() -> AuthorizerTypeType:
    return "CUSTOM_JWT"
```

```python
# AuthorizerTypeType definition
AuthorizerTypeType = Literal[
    "CUSTOM_JWT",
]
```
## BrowserNetworkModeType

```python
# BrowserNetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BrowserNetworkModeType

def get_value() -> BrowserNetworkModeType:
    return "PUBLIC"
```

```python
# BrowserNetworkModeType definition
BrowserNetworkModeType = Literal[
    "PUBLIC",
]
```
## BrowserStatusType

```python
# BrowserStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BrowserStatusType

def get_value() -> BrowserStatusType:
    return "CREATE_FAILED"
```

```python
# BrowserStatusType definition
BrowserStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "READY",
]
```
## CodeInterpreterNetworkModeType

```python
# CodeInterpreterNetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CodeInterpreterNetworkModeType

def get_value() -> CodeInterpreterNetworkModeType:
    return "PUBLIC"
```

```python
# CodeInterpreterNetworkModeType definition
CodeInterpreterNetworkModeType = Literal[
    "PUBLIC",
    "SANDBOX",
]
```
## CodeInterpreterStatusType

```python
# CodeInterpreterStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CodeInterpreterStatusType

def get_value() -> CodeInterpreterStatusType:
    return "CREATE_FAILED"
```

```python
# CodeInterpreterStatusType definition
CodeInterpreterStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "READY",
]
```
## CredentialProviderTypeType

```python
# CredentialProviderTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CredentialProviderTypeType

def get_value() -> CredentialProviderTypeType:
    return "API_KEY"
```

```python
# CredentialProviderTypeType definition
CredentialProviderTypeType = Literal[
    "API_KEY",
    "GATEWAY_IAM_ROLE",
    "OAUTH",
]
```
## CredentialProviderVendorTypeType

```python
# CredentialProviderVendorTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CredentialProviderVendorTypeType

def get_value() -> CredentialProviderVendorTypeType:
    return "CustomOauth2"
```

```python
# CredentialProviderVendorTypeType definition
CredentialProviderVendorTypeType = Literal[
    "CustomOauth2",
    "GithubOauth2",
    "GoogleOauth2",
    "MicrosoftOauth2",
    "SalesforceOauth2",
    "SlackOauth2",
]
```
## ExceptionLevelType

```python
# ExceptionLevelType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ExceptionLevelType

def get_value() -> ExceptionLevelType:
    return "DEBUG"
```

```python
# ExceptionLevelType definition
ExceptionLevelType = Literal[
    "DEBUG",
]
```
## GatewayProtocolTypeType

```python
# GatewayProtocolTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayProtocolTypeType

def get_value() -> GatewayProtocolTypeType:
    return "MCP"
```

```python
# GatewayProtocolTypeType definition
GatewayProtocolTypeType = Literal[
    "MCP",
]
```
## GatewayStatusType

```python
# GatewayStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayStatusType

def get_value() -> GatewayStatusType:
    return "CREATING"
```

```python
# GatewayStatusType definition
GatewayStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "READY",
    "UPDATE_UNSUCCESSFUL",
    "UPDATING",
]
```
## KeyTypeType

```python
# KeyTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "CustomerManagedKey"
```

```python
# KeyTypeType definition
KeyTypeType = Literal[
    "CustomerManagedKey",
    "ServiceManagedKey",
]
```
## ListAgentRuntimeEndpointsPaginatorName

```python
# ListAgentRuntimeEndpointsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimeEndpointsPaginatorName

def get_value() -> ListAgentRuntimeEndpointsPaginatorName:
    return "list_agent_runtime_endpoints"
```

```python
# ListAgentRuntimeEndpointsPaginatorName definition
ListAgentRuntimeEndpointsPaginatorName = Literal[
    "list_agent_runtime_endpoints",
]
```
## ListAgentRuntimeVersionsPaginatorName

```python
# ListAgentRuntimeVersionsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimeVersionsPaginatorName

def get_value() -> ListAgentRuntimeVersionsPaginatorName:
    return "list_agent_runtime_versions"
```

```python
# ListAgentRuntimeVersionsPaginatorName definition
ListAgentRuntimeVersionsPaginatorName = Literal[
    "list_agent_runtime_versions",
]
```
## ListAgentRuntimesPaginatorName

```python
# ListAgentRuntimesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimesPaginatorName

def get_value() -> ListAgentRuntimesPaginatorName:
    return "list_agent_runtimes"
```

```python
# ListAgentRuntimesPaginatorName definition
ListAgentRuntimesPaginatorName = Literal[
    "list_agent_runtimes",
]
```
## ListApiKeyCredentialProvidersPaginatorName

```python
# ListApiKeyCredentialProvidersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListApiKeyCredentialProvidersPaginatorName

def get_value() -> ListApiKeyCredentialProvidersPaginatorName:
    return "list_api_key_credential_providers"
```

```python
# ListApiKeyCredentialProvidersPaginatorName definition
ListApiKeyCredentialProvidersPaginatorName = Literal[
    "list_api_key_credential_providers",
]
```
## ListBrowsersPaginatorName

```python
# ListBrowsersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListBrowsersPaginatorName

def get_value() -> ListBrowsersPaginatorName:
    return "list_browsers"
```

```python
# ListBrowsersPaginatorName definition
ListBrowsersPaginatorName = Literal[
    "list_browsers",
]
```
## ListCodeInterpretersPaginatorName

```python
# ListCodeInterpretersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListCodeInterpretersPaginatorName

def get_value() -> ListCodeInterpretersPaginatorName:
    return "list_code_interpreters"
```

```python
# ListCodeInterpretersPaginatorName definition
ListCodeInterpretersPaginatorName = Literal[
    "list_code_interpreters",
]
```
## ListGatewayTargetsPaginatorName

```python
# ListGatewayTargetsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListGatewayTargetsPaginatorName

def get_value() -> ListGatewayTargetsPaginatorName:
    return "list_gateway_targets"
```

```python
# ListGatewayTargetsPaginatorName definition
ListGatewayTargetsPaginatorName = Literal[
    "list_gateway_targets",
]
```
## ListGatewaysPaginatorName

```python
# ListGatewaysPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListGatewaysPaginatorName

def get_value() -> ListGatewaysPaginatorName:
    return "list_gateways"
```

```python
# ListGatewaysPaginatorName definition
ListGatewaysPaginatorName = Literal[
    "list_gateways",
]
```
## ListMemoriesPaginatorName

```python
# ListMemoriesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListMemoriesPaginatorName

def get_value() -> ListMemoriesPaginatorName:
    return "list_memories"
```

```python
# ListMemoriesPaginatorName definition
ListMemoriesPaginatorName = Literal[
    "list_memories",
]
```
## ListOauth2CredentialProvidersPaginatorName

```python
# ListOauth2CredentialProvidersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListOauth2CredentialProvidersPaginatorName

def get_value() -> ListOauth2CredentialProvidersPaginatorName:
    return "list_oauth2_credential_providers"
```

```python
# ListOauth2CredentialProvidersPaginatorName definition
ListOauth2CredentialProvidersPaginatorName = Literal[
    "list_oauth2_credential_providers",
]
```
## ListWorkloadIdentitiesPaginatorName

```python
# ListWorkloadIdentitiesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListWorkloadIdentitiesPaginatorName

def get_value() -> ListWorkloadIdentitiesPaginatorName:
    return "list_workload_identities"
```

```python
# ListWorkloadIdentitiesPaginatorName definition
ListWorkloadIdentitiesPaginatorName = Literal[
    "list_workload_identities",
]
```
## MemoryCreatedWaiterName

```python
# MemoryCreatedWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryCreatedWaiterName

def get_value() -> MemoryCreatedWaiterName:
    return "memory_created"
```

```python
# MemoryCreatedWaiterName definition
MemoryCreatedWaiterName = Literal[
    "memory_created",
]
```
## MemoryStatusType

```python
# MemoryStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStatusType

def get_value() -> MemoryStatusType:
    return "ACTIVE"
```

```python
# MemoryStatusType definition
MemoryStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## MemoryStrategyStatusType

```python
# MemoryStrategyStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStrategyStatusType

def get_value() -> MemoryStrategyStatusType:
    return "ACTIVE"
```

```python
# MemoryStrategyStatusType definition
MemoryStrategyStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## MemoryStrategyTypeType

```python
# MemoryStrategyTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStrategyTypeType

def get_value() -> MemoryStrategyTypeType:
    return "CUSTOM"
```

```python
# MemoryStrategyTypeType definition
MemoryStrategyTypeType = Literal[
    "CUSTOM",
    "SEMANTIC",
    "SUMMARIZATION",
    "USER_PREFERENCE",
]
```
## NetworkModeType

```python
# NetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import NetworkModeType

def get_value() -> NetworkModeType:
    return "PUBLIC"
```

```python
# NetworkModeType definition
NetworkModeType = Literal[
    "PUBLIC",
]
```
## OverrideTypeType

```python
# OverrideTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import OverrideTypeType

def get_value() -> OverrideTypeType:
    return "SEMANTIC_OVERRIDE"
```

```python
# OverrideTypeType definition
OverrideTypeType = Literal[
    "SEMANTIC_OVERRIDE",
    "SUMMARY_OVERRIDE",
    "USER_PREFERENCE_OVERRIDE",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "CUSTOM"
```

```python
# ResourceTypeType definition
ResourceTypeType = Literal[
    "CUSTOM",
    "SYSTEM",
]
```
## SchemaTypeType

```python
# SchemaTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import SchemaTypeType

def get_value() -> SchemaTypeType:
    return "array"
```

```python
# SchemaTypeType definition
SchemaTypeType = Literal[
    "array",
    "boolean",
    "integer",
    "number",
    "object",
    "string",
]
```
## SearchTypeType

```python
# SearchTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import SearchTypeType

def get_value() -> SearchTypeType:
    return "SEMANTIC"
```

```python
# SearchTypeType definition
SearchTypeType = Literal[
    "SEMANTIC",
]
```
## ServerProtocolType

```python
# ServerProtocolType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ServerProtocolType

def get_value() -> ServerProtocolType:
    return "HTTP"
```

```python
# ServerProtocolType definition
ServerProtocolType = Literal[
    "HTTP",
    "MCP",
]
```
## TargetStatusType

```python
# TargetStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import TargetStatusType

def get_value() -> TargetStatusType:
    return "CREATING"
```

```python
# TargetStatusType definition
TargetStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "READY",
    "UPDATE_UNSUCCESSFUL",
    "UPDATING",
]
```
## BedrockAgentCoreControlPlaneFrontingLayerServiceName

```python
# BedrockAgentCoreControlPlaneFrontingLayerServiceName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BedrockAgentCoreControlPlaneFrontingLayerServiceName

def get_value() -> BedrockAgentCoreControlPlaneFrontingLayerServiceName:
    return "bedrock-agentcore-control"
```

```python
# BedrockAgentCoreControlPlaneFrontingLayerServiceName definition
BedrockAgentCoreControlPlaneFrontingLayerServiceName = Literal[
    "bedrock-agentcore-control",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ServiceName

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
    "apptest",
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
    "mpa",
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
    "odb",
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
    "simspaceweaver",
    "sms",
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
from types_aiobotocore_bedrock_agentcore_control.literals import ResourceServiceName

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
from types_aiobotocore_bedrock_agentcore_control.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_agent_runtime_endpoints"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_agent_runtime_endpoints",
    "list_agent_runtime_versions",
    "list_agent_runtimes",
    "list_api_key_credential_providers",
    "list_browsers",
    "list_code_interpreters",
    "list_gateway_targets",
    "list_gateways",
    "list_memories",
    "list_oauth2_credential_providers",
    "list_workload_identities",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import WaiterName

def get_value() -> WaiterName:
    return "memory_created"
```

```python
# WaiterName definition
WaiterName = Literal[
    "memory_created",
]
```
