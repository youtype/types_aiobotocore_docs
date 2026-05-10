# Literals

> [Index](../README.md) > [SecurityAgent](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SecurityAgent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#securityagent)
    type annotations stubs module [types-aiobotocore-securityagent](https://pypi.org/project/types-aiobotocore-securityagent/).

## AccessTypeType

```python
# AccessTypeType usage example
from types_aiobotocore_securityagent.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "PRIVATE"
```

```python
# AccessTypeType definition
AccessTypeType = Literal[
    "PRIVATE",
    "PUBLIC",
]
```
## ArtifactTypeType

```python
# ArtifactTypeType usage example
from types_aiobotocore_securityagent.literals import ArtifactTypeType

def get_value() -> ArtifactTypeType:
    return "DOC"
```

```python
# ArtifactTypeType definition
ArtifactTypeType = Literal[
    "DOC",
    "DOCX",
    "JPEG",
    "JSON",
    "MD",
    "PDF",
    "PNG",
    "TXT",
    "YAML",
]
```
## AuthenticationProviderTypeType

```python
# AuthenticationProviderTypeType usage example
from types_aiobotocore_securityagent.literals import AuthenticationProviderTypeType

def get_value() -> AuthenticationProviderTypeType:
    return "AWS_IAM_ROLE"
```

```python
# AuthenticationProviderTypeType definition
AuthenticationProviderTypeType = Literal[
    "AWS_IAM_ROLE",
    "AWS_INTERNAL",
    "AWS_LAMBDA",
    "SECRETS_MANAGER",
]
```
## CodeRemediationStrategyType

```python
# CodeRemediationStrategyType usage example
from types_aiobotocore_securityagent.literals import CodeRemediationStrategyType

def get_value() -> CodeRemediationStrategyType:
    return "AUTOMATIC"
```

```python
# CodeRemediationStrategyType definition
CodeRemediationStrategyType = Literal[
    "AUTOMATIC",
    "DISABLED",
]
```
## CodeRemediationTaskStatusType

```python
# CodeRemediationTaskStatusType usage example
from types_aiobotocore_securityagent.literals import CodeRemediationTaskStatusType

def get_value() -> CodeRemediationTaskStatusType:
    return "COMPLETED"
```

```python
# CodeRemediationTaskStatusType definition
CodeRemediationTaskStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## ConfidenceLevelType

```python
# ConfidenceLevelType usage example
from types_aiobotocore_securityagent.literals import ConfidenceLevelType

def get_value() -> ConfidenceLevelType:
    return "FALSE_POSITIVE"
```

```python
# ConfidenceLevelType definition
ConfidenceLevelType = Literal[
    "FALSE_POSITIVE",
    "HIGH",
    "LOW",
    "MEDIUM",
    "UNCONFIRMED",
]
```
## ContextTypeType

```python
# ContextTypeType usage example
from types_aiobotocore_securityagent.literals import ContextTypeType

def get_value() -> ContextTypeType:
    return "CLIENT_ERROR"
```

```python
# ContextTypeType definition
ContextTypeType = Literal[
    "CLIENT_ERROR",
    "ERROR",
    "INFO",
    "WARNING",
]
```
## DNSRecordTypeType

```python
# DNSRecordTypeType usage example
from types_aiobotocore_securityagent.literals import DNSRecordTypeType

def get_value() -> DNSRecordTypeType:
    return "TXT"
```

```python
# DNSRecordTypeType definition
DNSRecordTypeType = Literal[
    "TXT",
]
```
## DomainVerificationMethodType

```python
# DomainVerificationMethodType usage example
from types_aiobotocore_securityagent.literals import DomainVerificationMethodType

def get_value() -> DomainVerificationMethodType:
    return "DNS_TXT"
```

```python
# DomainVerificationMethodType definition
DomainVerificationMethodType = Literal[
    "DNS_TXT",
    "HTTP_ROUTE",
    "PRIVATE_VPC",
]
```
## ErrorCodeType

```python
# ErrorCodeType usage example
from types_aiobotocore_securityagent.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "CLIENT_ERROR"
```

```python
# ErrorCodeType definition
ErrorCodeType = Literal[
    "CLIENT_ERROR",
    "INTERNAL_ERROR",
    "STOPPED_BY_USER",
]
```
## FindingStatusType

```python
# FindingStatusType usage example
from types_aiobotocore_securityagent.literals import FindingStatusType

def get_value() -> FindingStatusType:
    return "ACCEPTED"
```

```python
# FindingStatusType definition
FindingStatusType = Literal[
    "ACCEPTED",
    "ACTIVE",
    "FALSE_POSITIVE",
    "RESOLVED",
]
```
## JobStatusType

```python
# JobStatusType usage example
from types_aiobotocore_securityagent.literals import JobStatusType

def get_value() -> JobStatusType:
    return "COMPLETED"
```

```python
# JobStatusType definition
JobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "STOPPED",
    "STOPPING",
]
```
## ListAgentSpacesPaginatorName

```python
# ListAgentSpacesPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListAgentSpacesPaginatorName

def get_value() -> ListAgentSpacesPaginatorName:
    return "list_agent_spaces"
```

```python
# ListAgentSpacesPaginatorName definition
ListAgentSpacesPaginatorName = Literal[
    "list_agent_spaces",
]
```
## ListApplicationsPaginatorName

```python
# ListApplicationsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python
# ListApplicationsPaginatorName definition
ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListArtifactsPaginatorName

```python
# ListArtifactsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListArtifactsPaginatorName

def get_value() -> ListArtifactsPaginatorName:
    return "list_artifacts"
```

```python
# ListArtifactsPaginatorName definition
ListArtifactsPaginatorName = Literal[
    "list_artifacts",
]
```
## ListDiscoveredEndpointsPaginatorName

```python
# ListDiscoveredEndpointsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListDiscoveredEndpointsPaginatorName

def get_value() -> ListDiscoveredEndpointsPaginatorName:
    return "list_discovered_endpoints"
```

```python
# ListDiscoveredEndpointsPaginatorName definition
ListDiscoveredEndpointsPaginatorName = Literal[
    "list_discovered_endpoints",
]
```
## ListFindingsPaginatorName

```python
# ListFindingsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListFindingsPaginatorName

def get_value() -> ListFindingsPaginatorName:
    return "list_findings"
```

```python
# ListFindingsPaginatorName definition
ListFindingsPaginatorName = Literal[
    "list_findings",
]
```
## ListIntegratedResourcesPaginatorName

```python
# ListIntegratedResourcesPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListIntegratedResourcesPaginatorName

def get_value() -> ListIntegratedResourcesPaginatorName:
    return "list_integrated_resources"
```

```python
# ListIntegratedResourcesPaginatorName definition
ListIntegratedResourcesPaginatorName = Literal[
    "list_integrated_resources",
]
```
## ListIntegrationsPaginatorName

```python
# ListIntegrationsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListIntegrationsPaginatorName

def get_value() -> ListIntegrationsPaginatorName:
    return "list_integrations"
```

```python
# ListIntegrationsPaginatorName definition
ListIntegrationsPaginatorName = Literal[
    "list_integrations",
]
```
## ListMembershipsPaginatorName

```python
# ListMembershipsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListMembershipsPaginatorName

def get_value() -> ListMembershipsPaginatorName:
    return "list_memberships"
```

```python
# ListMembershipsPaginatorName definition
ListMembershipsPaginatorName = Literal[
    "list_memberships",
]
```
## ListPentestJobTasksPaginatorName

```python
# ListPentestJobTasksPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListPentestJobTasksPaginatorName

def get_value() -> ListPentestJobTasksPaginatorName:
    return "list_pentest_job_tasks"
```

```python
# ListPentestJobTasksPaginatorName definition
ListPentestJobTasksPaginatorName = Literal[
    "list_pentest_job_tasks",
]
```
## ListPentestJobsForPentestPaginatorName

```python
# ListPentestJobsForPentestPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListPentestJobsForPentestPaginatorName

def get_value() -> ListPentestJobsForPentestPaginatorName:
    return "list_pentest_jobs_for_pentest"
```

```python
# ListPentestJobsForPentestPaginatorName definition
ListPentestJobsForPentestPaginatorName = Literal[
    "list_pentest_jobs_for_pentest",
]
```
## ListPentestsPaginatorName

```python
# ListPentestsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListPentestsPaginatorName

def get_value() -> ListPentestsPaginatorName:
    return "list_pentests"
```

```python
# ListPentestsPaginatorName definition
ListPentestsPaginatorName = Literal[
    "list_pentests",
]
```
## ListTargetDomainsPaginatorName

```python
# ListTargetDomainsPaginatorName usage example
from types_aiobotocore_securityagent.literals import ListTargetDomainsPaginatorName

def get_value() -> ListTargetDomainsPaginatorName:
    return "list_target_domains"
```

```python
# ListTargetDomainsPaginatorName definition
ListTargetDomainsPaginatorName = Literal[
    "list_target_domains",
]
```
## LogTypeType

```python
# LogTypeType usage example
from types_aiobotocore_securityagent.literals import LogTypeType

def get_value() -> LogTypeType:
    return "CLOUDWATCH"
```

```python
# LogTypeType definition
LogTypeType = Literal[
    "CLOUDWATCH",
]
```
## MembershipTypeFilterType

```python
# MembershipTypeFilterType usage example
from types_aiobotocore_securityagent.literals import MembershipTypeFilterType

def get_value() -> MembershipTypeFilterType:
    return "ALL"
```

```python
# MembershipTypeFilterType definition
MembershipTypeFilterType = Literal[
    "ALL",
    "USER",
]
```
## MembershipTypeType

```python
# MembershipTypeType usage example
from types_aiobotocore_securityagent.literals import MembershipTypeType

def get_value() -> MembershipTypeType:
    return "USER"
```

```python
# MembershipTypeType definition
MembershipTypeType = Literal[
    "USER",
]
```
## NetworkTrafficRuleEffectType

```python
# NetworkTrafficRuleEffectType usage example
from types_aiobotocore_securityagent.literals import NetworkTrafficRuleEffectType

def get_value() -> NetworkTrafficRuleEffectType:
    return "ALLOW"
```

```python
# NetworkTrafficRuleEffectType definition
NetworkTrafficRuleEffectType = Literal[
    "ALLOW",
    "DENY",
]
```
## NetworkTrafficRuleTypeType

```python
# NetworkTrafficRuleTypeType usage example
from types_aiobotocore_securityagent.literals import NetworkTrafficRuleTypeType

def get_value() -> NetworkTrafficRuleTypeType:
    return "URL"
```

```python
# NetworkTrafficRuleTypeType definition
NetworkTrafficRuleTypeType = Literal[
    "URL",
]
```
## ProviderType

```python
# ProviderType usage example
from types_aiobotocore_securityagent.literals import ProviderType

def get_value() -> ProviderType:
    return "GITHUB"
```

```python
# ProviderType definition
ProviderType = Literal[
    "GITHUB",
]
```
## ProviderTypeType

```python
# ProviderTypeType usage example
from types_aiobotocore_securityagent.literals import ProviderTypeType

def get_value() -> ProviderTypeType:
    return "DOCUMENTATION"
```

```python
# ProviderTypeType definition
ProviderTypeType = Literal[
    "DOCUMENTATION",
    "SOURCE_CODE",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example
from types_aiobotocore_securityagent.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "CODE_REPOSITORY"
```

```python
# ResourceTypeType definition
ResourceTypeType = Literal[
    "CODE_REPOSITORY",
]
```
## RiskLevelType

```python
# RiskLevelType usage example
from types_aiobotocore_securityagent.literals import RiskLevelType

def get_value() -> RiskLevelType:
    return "CRITICAL"
```

```python
# RiskLevelType definition
RiskLevelType = Literal[
    "CRITICAL",
    "HIGH",
    "INFORMATIONAL",
    "LOW",
    "MEDIUM",
    "UNKNOWN",
]
```
## RiskTypeType

```python
# RiskTypeType usage example
from types_aiobotocore_securityagent.literals import RiskTypeType

def get_value() -> RiskTypeType:
    return "ARBITRARY_FILE_UPLOAD"
```

```python
# RiskTypeType definition
RiskTypeType = Literal[
    "ARBITRARY_FILE_UPLOAD",
    "BUSINESS_LOGIC_VULNERABILITIES",
    "CODE_INJECTION",
    "COMMAND_INJECTION",
    "CROSS_SITE_SCRIPTING",
    "CRYPTOGRAPHIC_VULNERABILITIES",
    "DATABASE_ACCESS",
    "DATABASE_MODIFICATION",
    "DEFAULT_CREDENTIALS",
    "DENIAL_OF_SERVICE",
    "FILE_ACCESS",
    "FILE_CREATION",
    "FILE_DELETION",
    "GRAPHQL_VULNERABILITIES",
    "INFORMATION_DISCLOSURE",
    "INSECURE_DESERIALIZATION",
    "INSECURE_DIRECT_OBJECT_REFERENCE",
    "JSON_WEB_TOKEN_VULNERABILITIES",
    "LOCAL_FILE_INCLUSION",
    "OTHER",
    "OUTBOUND_SERVICE_REQUEST",
    "PATH_TRAVERSAL",
    "PRIVILEGE_ESCALATION",
    "SERVER_SIDE_REQUEST_FORGERY",
    "SERVER_SIDE_TEMPLATE_INJECTION",
    "SQL_INJECTION",
    "UNKNOWN",
    "XML_EXTERNAL_ENTITY",
]
```
## StepNameType

```python
# StepNameType usage example
from types_aiobotocore_securityagent.literals import StepNameType

def get_value() -> StepNameType:
    return "FINALIZING"
```

```python
# StepNameType definition
StepNameType = Literal[
    "FINALIZING",
    "PENTEST",
    "PREFLIGHT",
    "STATIC_ANALYSIS",
]
```
## StepStatusType

```python
# StepStatusType usage example
from types_aiobotocore_securityagent.literals import StepStatusType

def get_value() -> StepStatusType:
    return "COMPLETED"
```

```python
# StepStatusType definition
StepStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "NOT_STARTED",
    "STOPPED",
]
```
## TargetDomainStatusType

```python
# TargetDomainStatusType usage example
from types_aiobotocore_securityagent.literals import TargetDomainStatusType

def get_value() -> TargetDomainStatusType:
    return "FAILED"
```

```python
# TargetDomainStatusType definition
TargetDomainStatusType = Literal[
    "FAILED",
    "PENDING",
    "UNREACHABLE",
    "VERIFIED",
]
```
## TaskExecutionStatusType

```python
# TaskExecutionStatusType usage example
from types_aiobotocore_securityagent.literals import TaskExecutionStatusType

def get_value() -> TaskExecutionStatusType:
    return "ABORTED"
```

```python
# TaskExecutionStatusType definition
TaskExecutionStatusType = Literal[
    "ABORTED",
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
    "INTERNAL_ERROR",
]
```
## UserRoleType

```python
# UserRoleType usage example
from types_aiobotocore_securityagent.literals import UserRoleType

def get_value() -> UserRoleType:
    return "MEMBER"
```

```python
# UserRoleType definition
UserRoleType = Literal[
    "MEMBER",
]
```
## SecurityAgentServiceName

```python
# SecurityAgentServiceName usage example
from types_aiobotocore_securityagent.literals import SecurityAgentServiceName

def get_value() -> SecurityAgentServiceName:
    return "securityagent"
```

```python
# SecurityAgentServiceName definition
SecurityAgentServiceName = Literal[
    "securityagent",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_securityagent.literals import ServiceName

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
    "connecthealth",
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
    "devops-agent",
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
    "elementalinference",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
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
    "interconnect",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-managed-integrations",
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
    "marketplace-discovery",
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
    "s3files",
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
    "securityagent",
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
    "signer-data",
    "signin",
    "simpledbv2",
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
    "sustainability",
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
    "uxc",
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
from types_aiobotocore_securityagent.literals import ResourceServiceName

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
from types_aiobotocore_securityagent.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_agent_spaces"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_agent_spaces",
    "list_applications",
    "list_artifacts",
    "list_discovered_endpoints",
    "list_findings",
    "list_integrated_resources",
    "list_integrations",
    "list_memberships",
    "list_pentest_job_tasks",
    "list_pentest_jobs_for_pentest",
    "list_pentests",
    "list_target_domains",
]
```
