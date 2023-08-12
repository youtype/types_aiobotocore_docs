# Literals

> [Index](../README.md) > [ResilienceHub](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## AlarmTypeType

```python
# AlarmTypeType usage example

from types_aiobotocore_resiliencehub.literals import AlarmTypeType

def get_value() -> AlarmTypeType:
    return "Canary"
```

```python
# AlarmTypeType definition

AlarmTypeType = Literal[
    "Canary",
    "Composite",
    "Event",
    "Logs",
    "Metric",
]
```
## AppAssessmentScheduleTypeType

```python
# AppAssessmentScheduleTypeType usage example

from types_aiobotocore_resiliencehub.literals import AppAssessmentScheduleTypeType

def get_value() -> AppAssessmentScheduleTypeType:
    return "Daily"
```

```python
# AppAssessmentScheduleTypeType definition

AppAssessmentScheduleTypeType = Literal[
    "Daily",
    "Disabled",
]
```
## AppComplianceStatusTypeType

```python
# AppComplianceStatusTypeType usage example

from types_aiobotocore_resiliencehub.literals import AppComplianceStatusTypeType

def get_value() -> AppComplianceStatusTypeType:
    return "ChangesDetected"
```

```python
# AppComplianceStatusTypeType definition

AppComplianceStatusTypeType = Literal[
    "ChangesDetected",
    "NotAssessed",
    "PolicyBreached",
    "PolicyMet",
]
```
## AppDriftStatusTypeType

```python
# AppDriftStatusTypeType usage example

from types_aiobotocore_resiliencehub.literals import AppDriftStatusTypeType

def get_value() -> AppDriftStatusTypeType:
    return "Detected"
```

```python
# AppDriftStatusTypeType definition

AppDriftStatusTypeType = Literal[
    "Detected",
    "NotChecked",
    "NotDetected",
]
```
## AppStatusTypeType

```python
# AppStatusTypeType usage example

from types_aiobotocore_resiliencehub.literals import AppStatusTypeType

def get_value() -> AppStatusTypeType:
    return "Active"
```

```python
# AppStatusTypeType definition

AppStatusTypeType = Literal[
    "Active",
    "Deleting",
]
```
## AssessmentInvokerType

```python
# AssessmentInvokerType usage example

from types_aiobotocore_resiliencehub.literals import AssessmentInvokerType

def get_value() -> AssessmentInvokerType:
    return "System"
```

```python
# AssessmentInvokerType definition

AssessmentInvokerType = Literal[
    "System",
    "User",
]
```
## AssessmentStatusType

```python
# AssessmentStatusType usage example

from types_aiobotocore_resiliencehub.literals import AssessmentStatusType

def get_value() -> AssessmentStatusType:
    return "Failed"
```

```python
# AssessmentStatusType definition

AssessmentStatusType = Literal[
    "Failed",
    "InProgress",
    "Pending",
    "Success",
]
```
## ComplianceStatusType

```python
# ComplianceStatusType usage example

from types_aiobotocore_resiliencehub.literals import ComplianceStatusType

def get_value() -> ComplianceStatusType:
    return "PolicyBreached"
```

```python
# ComplianceStatusType definition

ComplianceStatusType = Literal[
    "PolicyBreached",
    "PolicyMet",
]
```
## ConfigRecommendationOptimizationTypeType

```python
# ConfigRecommendationOptimizationTypeType usage example

from types_aiobotocore_resiliencehub.literals import ConfigRecommendationOptimizationTypeType

def get_value() -> ConfigRecommendationOptimizationTypeType:
    return "BestAZRecovery"
```

```python
# ConfigRecommendationOptimizationTypeType definition

ConfigRecommendationOptimizationTypeType = Literal[
    "BestAttainable",
    "BestAZRecovery",
    "BestRegionRecovery",
    "LeastChange",
    "LeastCost",
    "LeastErrors",
]
```
## CostFrequencyType

```python
# CostFrequencyType usage example

from types_aiobotocore_resiliencehub.literals import CostFrequencyType

def get_value() -> CostFrequencyType:
    return "Daily"
```

```python
# CostFrequencyType definition

CostFrequencyType = Literal[
    "Daily",
    "Hourly",
    "Monthly",
    "Yearly",
]
```
## DataLocationConstraintType

```python
# DataLocationConstraintType usage example

from types_aiobotocore_resiliencehub.literals import DataLocationConstraintType

def get_value() -> DataLocationConstraintType:
    return "AnyLocation"
```

```python
# DataLocationConstraintType definition

DataLocationConstraintType = Literal[
    "AnyLocation",
    "SameContinent",
    "SameCountry",
]
```
## DifferenceTypeType

```python
# DifferenceTypeType usage example

from types_aiobotocore_resiliencehub.literals import DifferenceTypeType

def get_value() -> DifferenceTypeType:
    return "NotEqual"
```

```python
# DifferenceTypeType definition

DifferenceTypeType = Literal[
    "NotEqual",
]
```
## DisruptionTypeType

```python
# DisruptionTypeType usage example

from types_aiobotocore_resiliencehub.literals import DisruptionTypeType

def get_value() -> DisruptionTypeType:
    return "AZ"
```

```python
# DisruptionTypeType definition

DisruptionTypeType = Literal[
    "AZ",
    "Hardware",
    "Region",
    "Software",
]
```
## DriftStatusType

```python
# DriftStatusType usage example

from types_aiobotocore_resiliencehub.literals import DriftStatusType

def get_value() -> DriftStatusType:
    return "Detected"
```

```python
# DriftStatusType definition

DriftStatusType = Literal[
    "Detected",
    "NotChecked",
    "NotDetected",
]
```
## DriftTypeType

```python
# DriftTypeType usage example

from types_aiobotocore_resiliencehub.literals import DriftTypeType

def get_value() -> DriftTypeType:
    return "ApplicationCompliance"
```

```python
# DriftTypeType definition

DriftTypeType = Literal[
    "ApplicationCompliance",
]
```
## EstimatedCostTierType

```python
# EstimatedCostTierType usage example

from types_aiobotocore_resiliencehub.literals import EstimatedCostTierType

def get_value() -> EstimatedCostTierType:
    return "L1"
```

```python
# EstimatedCostTierType definition

EstimatedCostTierType = Literal[
    "L1",
    "L2",
    "L3",
    "L4",
]
```
## EventTypeType

```python
# EventTypeType usage example

from types_aiobotocore_resiliencehub.literals import EventTypeType

def get_value() -> EventTypeType:
    return "DriftDetected"
```

```python
# EventTypeType definition

EventTypeType = Literal[
    "DriftDetected",
    "ScheduledAssessmentFailure",
]
```
## ExcludeRecommendationReasonType

```python
# ExcludeRecommendationReasonType usage example

from types_aiobotocore_resiliencehub.literals import ExcludeRecommendationReasonType

def get_value() -> ExcludeRecommendationReasonType:
    return "AlreadyImplemented"
```

```python
# ExcludeRecommendationReasonType definition

ExcludeRecommendationReasonType = Literal[
    "AlreadyImplemented",
    "ComplexityOfImplementation",
    "NotRelevant",
]
```
## HaArchitectureType

```python
# HaArchitectureType usage example

from types_aiobotocore_resiliencehub.literals import HaArchitectureType

def get_value() -> HaArchitectureType:
    return "BackupAndRestore"
```

```python
# HaArchitectureType definition

HaArchitectureType = Literal[
    "BackupAndRestore",
    "MultiSite",
    "NoRecoveryPlan",
    "PilotLight",
    "WarmStandby",
]
```
## PermissionModelTypeType

```python
# PermissionModelTypeType usage example

from types_aiobotocore_resiliencehub.literals import PermissionModelTypeType

def get_value() -> PermissionModelTypeType:
    return "LegacyIAMUser"
```

```python
# PermissionModelTypeType definition

PermissionModelTypeType = Literal[
    "LegacyIAMUser",
    "RoleBased",
]
```
## PhysicalIdentifierTypeType

```python
# PhysicalIdentifierTypeType usage example

from types_aiobotocore_resiliencehub.literals import PhysicalIdentifierTypeType

def get_value() -> PhysicalIdentifierTypeType:
    return "Arn"
```

```python
# PhysicalIdentifierTypeType definition

PhysicalIdentifierTypeType = Literal[
    "Arn",
    "Native",
]
```
## RecommendationComplianceStatusType

```python
# RecommendationComplianceStatusType usage example

from types_aiobotocore_resiliencehub.literals import RecommendationComplianceStatusType

def get_value() -> RecommendationComplianceStatusType:
    return "BreachedCanMeet"
```

```python
# RecommendationComplianceStatusType definition

RecommendationComplianceStatusType = Literal[
    "BreachedCanMeet",
    "BreachedUnattainable",
    "MetCanImprove",
]
```
## RecommendationTemplateStatusType

```python
# RecommendationTemplateStatusType usage example

from types_aiobotocore_resiliencehub.literals import RecommendationTemplateStatusType

def get_value() -> RecommendationTemplateStatusType:
    return "Failed"
```

```python
# RecommendationTemplateStatusType definition

RecommendationTemplateStatusType = Literal[
    "Failed",
    "InProgress",
    "Pending",
    "Success",
]
```
## RenderRecommendationTypeType

```python
# RenderRecommendationTypeType usage example

from types_aiobotocore_resiliencehub.literals import RenderRecommendationTypeType

def get_value() -> RenderRecommendationTypeType:
    return "Alarm"
```

```python
# RenderRecommendationTypeType definition

RenderRecommendationTypeType = Literal[
    "Alarm",
    "Sop",
    "Test",
]
```
## ResiliencyPolicyTierType

```python
# ResiliencyPolicyTierType usage example

from types_aiobotocore_resiliencehub.literals import ResiliencyPolicyTierType

def get_value() -> ResiliencyPolicyTierType:
    return "CoreServices"
```

```python
# ResiliencyPolicyTierType definition

ResiliencyPolicyTierType = Literal[
    "CoreServices",
    "Critical",
    "Important",
    "MissionCritical",
    "NonCritical",
    "NotApplicable",
]
```
## ResourceImportStatusTypeType

```python
# ResourceImportStatusTypeType usage example

from types_aiobotocore_resiliencehub.literals import ResourceImportStatusTypeType

def get_value() -> ResourceImportStatusTypeType:
    return "Failed"
```

```python
# ResourceImportStatusTypeType definition

ResourceImportStatusTypeType = Literal[
    "Failed",
    "InProgress",
    "Pending",
    "Success",
]
```
## ResourceImportStrategyTypeType

```python
# ResourceImportStrategyTypeType usage example

from types_aiobotocore_resiliencehub.literals import ResourceImportStrategyTypeType

def get_value() -> ResourceImportStrategyTypeType:
    return "AddOnly"
```

```python
# ResourceImportStrategyTypeType definition

ResourceImportStrategyTypeType = Literal[
    "AddOnly",
    "ReplaceAll",
]
```
## ResourceMappingTypeType

```python
# ResourceMappingTypeType usage example

from types_aiobotocore_resiliencehub.literals import ResourceMappingTypeType

def get_value() -> ResourceMappingTypeType:
    return "AppRegistryApp"
```

```python
# ResourceMappingTypeType definition

ResourceMappingTypeType = Literal[
    "AppRegistryApp",
    "CfnStack",
    "EKS",
    "Resource",
    "ResourceGroup",
    "Terraform",
]
```
## ResourceResolutionStatusTypeType

```python
# ResourceResolutionStatusTypeType usage example

from types_aiobotocore_resiliencehub.literals import ResourceResolutionStatusTypeType

def get_value() -> ResourceResolutionStatusTypeType:
    return "Failed"
```

```python
# ResourceResolutionStatusTypeType definition

ResourceResolutionStatusTypeType = Literal[
    "Failed",
    "InProgress",
    "Pending",
    "Success",
]
```
## ResourceSourceTypeType

```python
# ResourceSourceTypeType usage example

from types_aiobotocore_resiliencehub.literals import ResourceSourceTypeType

def get_value() -> ResourceSourceTypeType:
    return "AppTemplate"
```

```python
# ResourceSourceTypeType definition

ResourceSourceTypeType = Literal[
    "AppTemplate",
    "Discovered",
]
```
## SopServiceTypeType

```python
# SopServiceTypeType usage example

from types_aiobotocore_resiliencehub.literals import SopServiceTypeType

def get_value() -> SopServiceTypeType:
    return "SSM"
```

```python
# SopServiceTypeType definition

SopServiceTypeType = Literal[
    "SSM",
]
```
## TemplateFormatType

```python
# TemplateFormatType usage example

from types_aiobotocore_resiliencehub.literals import TemplateFormatType

def get_value() -> TemplateFormatType:
    return "CfnJson"
```

```python
# TemplateFormatType definition

TemplateFormatType = Literal[
    "CfnJson",
    "CfnYaml",
]
```
## TestRiskType

```python
# TestRiskType usage example

from types_aiobotocore_resiliencehub.literals import TestRiskType

def get_value() -> TestRiskType:
    return "High"
```

```python
# TestRiskType definition

TestRiskType = Literal[
    "High",
    "Medium",
    "Small",
]
```
## TestTypeType

```python
# TestTypeType usage example

from types_aiobotocore_resiliencehub.literals import TestTypeType

def get_value() -> TestTypeType:
    return "AZ"
```

```python
# TestTypeType definition

TestTypeType = Literal[
    "AZ",
    "Hardware",
    "Region",
    "Software",
]
```
## ResilienceHubServiceName

```python
# ResilienceHubServiceName usage example

from types_aiobotocore_resiliencehub.literals import ResilienceHubServiceName

def get_value() -> ResilienceHubServiceName:
    return "resiliencehub"
```

```python
# ResilienceHubServiceName definition

ResilienceHubServiceName = Literal[
    "resiliencehub",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_resiliencehub.literals import ServiceName

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

from types_aiobotocore_resiliencehub.literals import ResourceServiceName

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
## RegionName

```python
# RegionName usage example

from types_aiobotocore_resiliencehub.literals import RegionName

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
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
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
