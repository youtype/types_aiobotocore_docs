# Literals

> [Index](../README.md) > [WellArchitected](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## AccountJiraIssueManagementStatusType

```python
# AccountJiraIssueManagementStatusType usage example
from types_aiobotocore_wellarchitected.literals import AccountJiraIssueManagementStatusType

def get_value() -> AccountJiraIssueManagementStatusType:
    return "DISABLED"
```

```python
# AccountJiraIssueManagementStatusType definition
AccountJiraIssueManagementStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AdditionalResourceTypeType

```python
# AdditionalResourceTypeType usage example
from types_aiobotocore_wellarchitected.literals import AdditionalResourceTypeType

def get_value() -> AdditionalResourceTypeType:
    return "HELPFUL_RESOURCE"
```

```python
# AdditionalResourceTypeType definition
AdditionalResourceTypeType = Literal[
    "HELPFUL_RESOURCE",
    "IMPROVEMENT_PLAN",
]
```
## AnswerReasonType

```python
# AnswerReasonType usage example
from types_aiobotocore_wellarchitected.literals import AnswerReasonType

def get_value() -> AnswerReasonType:
    return "ARCHITECTURE_CONSTRAINTS"
```

```python
# AnswerReasonType definition
AnswerReasonType = Literal[
    "ARCHITECTURE_CONSTRAINTS",
    "BUSINESS_PRIORITIES",
    "NONE",
    "OTHER",
    "OUT_OF_SCOPE",
]
```
## CheckFailureReasonType

```python
# CheckFailureReasonType usage example
from types_aiobotocore_wellarchitected.literals import CheckFailureReasonType

def get_value() -> CheckFailureReasonType:
    return "ACCESS_DENIED"
```

```python
# CheckFailureReasonType definition
CheckFailureReasonType = Literal[
    "ACCESS_DENIED",
    "ASSUME_ROLE_ERROR",
    "PREMIUM_SUPPORT_REQUIRED",
    "UNKNOWN_ERROR",
]
```
## CheckProviderType

```python
# CheckProviderType usage example
from types_aiobotocore_wellarchitected.literals import CheckProviderType

def get_value() -> CheckProviderType:
    return "TRUSTED_ADVISOR"
```

```python
# CheckProviderType definition
CheckProviderType = Literal[
    "TRUSTED_ADVISOR",
]
```
## CheckStatusType

```python
# CheckStatusType usage example
from types_aiobotocore_wellarchitected.literals import CheckStatusType

def get_value() -> CheckStatusType:
    return "ERROR"
```

```python
# CheckStatusType definition
CheckStatusType = Literal[
    "ERROR",
    "FETCH_FAILED",
    "NOT_AVAILABLE",
    "OKAY",
    "WARNING",
]
```
## ChoiceReasonType

```python
# ChoiceReasonType usage example
from types_aiobotocore_wellarchitected.literals import ChoiceReasonType

def get_value() -> ChoiceReasonType:
    return "ARCHITECTURE_CONSTRAINTS"
```

```python
# ChoiceReasonType definition
ChoiceReasonType = Literal[
    "ARCHITECTURE_CONSTRAINTS",
    "BUSINESS_PRIORITIES",
    "NONE",
    "OTHER",
    "OUT_OF_SCOPE",
]
```
## ChoiceStatusType

```python
# ChoiceStatusType usage example
from types_aiobotocore_wellarchitected.literals import ChoiceStatusType

def get_value() -> ChoiceStatusType:
    return "NOT_APPLICABLE"
```

```python
# ChoiceStatusType definition
ChoiceStatusType = Literal[
    "NOT_APPLICABLE",
    "SELECTED",
    "UNSELECTED",
]
```
## DefinitionTypeType

```python
# DefinitionTypeType usage example
from types_aiobotocore_wellarchitected.literals import DefinitionTypeType

def get_value() -> DefinitionTypeType:
    return "APP_REGISTRY"
```

```python
# DefinitionTypeType definition
DefinitionTypeType = Literal[
    "APP_REGISTRY",
    "WORKLOAD_METADATA",
]
```
## DifferenceStatusType

```python
# DifferenceStatusType usage example
from types_aiobotocore_wellarchitected.literals import DifferenceStatusType

def get_value() -> DifferenceStatusType:
    return "DELETED"
```

```python
# DifferenceStatusType definition
DifferenceStatusType = Literal[
    "DELETED",
    "NEW",
    "UPDATED",
]
```
## DiscoveryIntegrationStatusType

```python
# DiscoveryIntegrationStatusType usage example
from types_aiobotocore_wellarchitected.literals import DiscoveryIntegrationStatusType

def get_value() -> DiscoveryIntegrationStatusType:
    return "DISABLED"
```

```python
# DiscoveryIntegrationStatusType definition
DiscoveryIntegrationStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ImportLensStatusType

```python
# ImportLensStatusType usage example
from types_aiobotocore_wellarchitected.literals import ImportLensStatusType

def get_value() -> ImportLensStatusType:
    return "COMPLETE"
```

```python
# ImportLensStatusType definition
ImportLensStatusType = Literal[
    "COMPLETE",
    "ERROR",
    "IN_PROGRESS",
]
```
## IntegratingServiceType

```python
# IntegratingServiceType usage example
from types_aiobotocore_wellarchitected.literals import IntegratingServiceType

def get_value() -> IntegratingServiceType:
    return "JIRA"
```

```python
# IntegratingServiceType definition
IntegratingServiceType = Literal[
    "JIRA",
]
```
## IntegrationStatusInputType

```python
# IntegrationStatusInputType usage example
from types_aiobotocore_wellarchitected.literals import IntegrationStatusInputType

def get_value() -> IntegrationStatusInputType:
    return "NOT_CONFIGURED"
```

```python
# IntegrationStatusInputType definition
IntegrationStatusInputType = Literal[
    "NOT_CONFIGURED",
]
```
## IntegrationStatusType

```python
# IntegrationStatusType usage example
from types_aiobotocore_wellarchitected.literals import IntegrationStatusType

def get_value() -> IntegrationStatusType:
    return "CONFIGURED"
```

```python
# IntegrationStatusType definition
IntegrationStatusType = Literal[
    "CONFIGURED",
    "NOT_CONFIGURED",
]
```
## IssueManagementTypeType

```python
# IssueManagementTypeType usage example
from types_aiobotocore_wellarchitected.literals import IssueManagementTypeType

def get_value() -> IssueManagementTypeType:
    return "AUTO"
```

```python
# IssueManagementTypeType definition
IssueManagementTypeType = Literal[
    "AUTO",
    "MANUAL",
]
```
## LensStatusType

```python
# LensStatusType usage example
from types_aiobotocore_wellarchitected.literals import LensStatusType

def get_value() -> LensStatusType:
    return "CURRENT"
```

```python
# LensStatusType definition
LensStatusType = Literal[
    "CURRENT",
    "DELETED",
    "DEPRECATED",
    "NOT_CURRENT",
    "UNSHARED",
]
```
## LensStatusTypeType

```python
# LensStatusTypeType usage example
from types_aiobotocore_wellarchitected.literals import LensStatusTypeType

def get_value() -> LensStatusTypeType:
    return "ALL"
```

```python
# LensStatusTypeType definition
LensStatusTypeType = Literal[
    "ALL",
    "DRAFT",
    "PUBLISHED",
]
```
## LensTypeType

```python
# LensTypeType usage example
from types_aiobotocore_wellarchitected.literals import LensTypeType

def get_value() -> LensTypeType:
    return "AWS_OFFICIAL"
```

```python
# LensTypeType definition
LensTypeType = Literal[
    "AWS_OFFICIAL",
    "CUSTOM_SELF",
    "CUSTOM_SHARED",
]
```
## MetricTypeType

```python
# MetricTypeType usage example
from types_aiobotocore_wellarchitected.literals import MetricTypeType

def get_value() -> MetricTypeType:
    return "WORKLOAD"
```

```python
# MetricTypeType definition
MetricTypeType = Literal[
    "WORKLOAD",
]
```
## NotificationTypeType

```python
# NotificationTypeType usage example
from types_aiobotocore_wellarchitected.literals import NotificationTypeType

def get_value() -> NotificationTypeType:
    return "LENS_VERSION_DEPRECATED"
```

```python
# NotificationTypeType definition
NotificationTypeType = Literal[
    "LENS_VERSION_DEPRECATED",
    "LENS_VERSION_UPGRADED",
]
```
## OrganizationSharingStatusType

```python
# OrganizationSharingStatusType usage example
from types_aiobotocore_wellarchitected.literals import OrganizationSharingStatusType

def get_value() -> OrganizationSharingStatusType:
    return "DISABLED"
```

```python
# OrganizationSharingStatusType definition
OrganizationSharingStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PermissionTypeType

```python
# PermissionTypeType usage example
from types_aiobotocore_wellarchitected.literals import PermissionTypeType

def get_value() -> PermissionTypeType:
    return "CONTRIBUTOR"
```

```python
# PermissionTypeType definition
PermissionTypeType = Literal[
    "CONTRIBUTOR",
    "READONLY",
]
```
## ProfileNotificationTypeType

```python
# ProfileNotificationTypeType usage example
from types_aiobotocore_wellarchitected.literals import ProfileNotificationTypeType

def get_value() -> ProfileNotificationTypeType:
    return "PROFILE_ANSWERS_UPDATED"
```

```python
# ProfileNotificationTypeType definition
ProfileNotificationTypeType = Literal[
    "PROFILE_ANSWERS_UPDATED",
    "PROFILE_DELETED",
]
```
## ProfileOwnerTypeType

```python
# ProfileOwnerTypeType usage example
from types_aiobotocore_wellarchitected.literals import ProfileOwnerTypeType

def get_value() -> ProfileOwnerTypeType:
    return "SELF"
```

```python
# ProfileOwnerTypeType definition
ProfileOwnerTypeType = Literal[
    "SELF",
    "SHARED",
]
```
## QuestionPriorityType

```python
# QuestionPriorityType usage example
from types_aiobotocore_wellarchitected.literals import QuestionPriorityType

def get_value() -> QuestionPriorityType:
    return "NONE"
```

```python
# QuestionPriorityType definition
QuestionPriorityType = Literal[
    "NONE",
    "PRIORITIZED",
]
```
## QuestionType

```python
# QuestionType usage example
from types_aiobotocore_wellarchitected.literals import QuestionType

def get_value() -> QuestionType:
    return "ANSWERED"
```

```python
# QuestionType definition
QuestionType = Literal[
    "ANSWERED",
    "UNANSWERED",
]
```
## QuestionTypeType

```python
# QuestionTypeType usage example
from types_aiobotocore_wellarchitected.literals import QuestionTypeType

def get_value() -> QuestionTypeType:
    return "NON_PRIORITIZED"
```

```python
# QuestionTypeType definition
QuestionTypeType = Literal[
    "NON_PRIORITIZED",
    "PRIORITIZED",
]
```
## ReportFormatType

```python
# ReportFormatType usage example
from types_aiobotocore_wellarchitected.literals import ReportFormatType

def get_value() -> ReportFormatType:
    return "JSON"
```

```python
# ReportFormatType definition
ReportFormatType = Literal[
    "JSON",
    "PDF",
]
```
## ReviewTemplateAnswerStatusType

```python
# ReviewTemplateAnswerStatusType usage example
from types_aiobotocore_wellarchitected.literals import ReviewTemplateAnswerStatusType

def get_value() -> ReviewTemplateAnswerStatusType:
    return "ANSWERED"
```

```python
# ReviewTemplateAnswerStatusType definition
ReviewTemplateAnswerStatusType = Literal[
    "ANSWERED",
    "UNANSWERED",
]
```
## ReviewTemplateUpdateStatusType

```python
# ReviewTemplateUpdateStatusType usage example
from types_aiobotocore_wellarchitected.literals import ReviewTemplateUpdateStatusType

def get_value() -> ReviewTemplateUpdateStatusType:
    return "CURRENT"
```

```python
# ReviewTemplateUpdateStatusType definition
ReviewTemplateUpdateStatusType = Literal[
    "CURRENT",
    "LENS_NOT_CURRENT",
]
```
## RiskType

```python
# RiskType usage example
from types_aiobotocore_wellarchitected.literals import RiskType

def get_value() -> RiskType:
    return "HIGH"
```

```python
# RiskType definition
RiskType = Literal[
    "HIGH",
    "MEDIUM",
    "NONE",
    "NOT_APPLICABLE",
    "UNANSWERED",
]
```
## ShareInvitationActionType

```python
# ShareInvitationActionType usage example
from types_aiobotocore_wellarchitected.literals import ShareInvitationActionType

def get_value() -> ShareInvitationActionType:
    return "ACCEPT"
```

```python
# ShareInvitationActionType definition
ShareInvitationActionType = Literal[
    "ACCEPT",
    "REJECT",
]
```
## ShareResourceTypeType

```python
# ShareResourceTypeType usage example
from types_aiobotocore_wellarchitected.literals import ShareResourceTypeType

def get_value() -> ShareResourceTypeType:
    return "LENS"
```

```python
# ShareResourceTypeType definition
ShareResourceTypeType = Literal[
    "LENS",
    "PROFILE",
    "TEMPLATE",
    "WORKLOAD",
]
```
## ShareStatusType

```python
# ShareStatusType usage example
from types_aiobotocore_wellarchitected.literals import ShareStatusType

def get_value() -> ShareStatusType:
    return "ACCEPTED"
```

```python
# ShareStatusType definition
ShareStatusType = Literal[
    "ACCEPTED",
    "ASSOCIATED",
    "ASSOCIATING",
    "EXPIRED",
    "FAILED",
    "PENDING",
    "REJECTED",
    "REVOKED",
]
```
## TrustedAdvisorIntegrationStatusType

```python
# TrustedAdvisorIntegrationStatusType usage example
from types_aiobotocore_wellarchitected.literals import TrustedAdvisorIntegrationStatusType

def get_value() -> TrustedAdvisorIntegrationStatusType:
    return "DISABLED"
```

```python
# TrustedAdvisorIntegrationStatusType definition
TrustedAdvisorIntegrationStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## WorkloadEnvironmentType

```python
# WorkloadEnvironmentType usage example
from types_aiobotocore_wellarchitected.literals import WorkloadEnvironmentType

def get_value() -> WorkloadEnvironmentType:
    return "PREPRODUCTION"
```

```python
# WorkloadEnvironmentType definition
WorkloadEnvironmentType = Literal[
    "PREPRODUCTION",
    "PRODUCTION",
]
```
## WorkloadImprovementStatusType

```python
# WorkloadImprovementStatusType usage example
from types_aiobotocore_wellarchitected.literals import WorkloadImprovementStatusType

def get_value() -> WorkloadImprovementStatusType:
    return "COMPLETE"
```

```python
# WorkloadImprovementStatusType definition
WorkloadImprovementStatusType = Literal[
    "COMPLETE",
    "IN_PROGRESS",
    "NOT_APPLICABLE",
    "NOT_STARTED",
    "RISK_ACKNOWLEDGED",
]
```
## WorkloadIssueManagementStatusType

```python
# WorkloadIssueManagementStatusType usage example
from types_aiobotocore_wellarchitected.literals import WorkloadIssueManagementStatusType

def get_value() -> WorkloadIssueManagementStatusType:
    return "DISABLED"
```

```python
# WorkloadIssueManagementStatusType definition
WorkloadIssueManagementStatusType = Literal[
    "DISABLED",
    "ENABLED",
    "INHERIT",
]
```
## WellArchitectedServiceName

```python
# WellArchitectedServiceName usage example
from types_aiobotocore_wellarchitected.literals import WellArchitectedServiceName

def get_value() -> WellArchitectedServiceName:
    return "wellarchitected"
```

```python
# WellArchitectedServiceName definition
WellArchitectedServiceName = Literal[
    "wellarchitected",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_wellarchitected.literals import ServiceName

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
from types_aiobotocore_wellarchitected.literals import ResourceServiceName

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
## RegionName

```python
# RegionName usage example
from types_aiobotocore_wellarchitected.literals import RegionName

def get_value() -> RegionName:
    return "ap-east-1"
```

```python
# RegionName definition
RegionName = Literal[
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
