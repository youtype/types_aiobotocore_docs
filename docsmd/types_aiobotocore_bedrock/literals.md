# Literals

> [Index](../README.md) > [Bedrock](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## ApplicationTypeType

```python
# ApplicationTypeType usage example

from types_aiobotocore_bedrock.literals import ApplicationTypeType

def get_value() -> ApplicationTypeType:
    return "ModelEvaluation"
```

```python
# ApplicationTypeType definition

ApplicationTypeType = Literal[
    "ModelEvaluation",
    "RagEvaluation",
]
```
## CommitmentDurationType

```python
# CommitmentDurationType usage example

from types_aiobotocore_bedrock.literals import CommitmentDurationType

def get_value() -> CommitmentDurationType:
    return "OneMonth"
```

```python
# CommitmentDurationType definition

CommitmentDurationType = Literal[
    "OneMonth",
    "SixMonths",
]
```
## CustomizationTypeType

```python
# CustomizationTypeType usage example

from types_aiobotocore_bedrock.literals import CustomizationTypeType

def get_value() -> CustomizationTypeType:
    return "CONTINUED_PRE_TRAINING"
```

```python
# CustomizationTypeType definition

CustomizationTypeType = Literal[
    "CONTINUED_PRE_TRAINING",
    "DISTILLATION",
    "FINE_TUNING",
]
```
## EvaluationJobStatusType

```python
# EvaluationJobStatusType usage example

from types_aiobotocore_bedrock.literals import EvaluationJobStatusType

def get_value() -> EvaluationJobStatusType:
    return "Completed"
```

```python
# EvaluationJobStatusType definition

EvaluationJobStatusType = Literal[
    "Completed",
    "Deleting",
    "Failed",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## EvaluationJobTypeType

```python
# EvaluationJobTypeType usage example

from types_aiobotocore_bedrock.literals import EvaluationJobTypeType

def get_value() -> EvaluationJobTypeType:
    return "Automated"
```

```python
# EvaluationJobTypeType definition

EvaluationJobTypeType = Literal[
    "Automated",
    "Human",
]
```
## EvaluationTaskTypeType

```python
# EvaluationTaskTypeType usage example

from types_aiobotocore_bedrock.literals import EvaluationTaskTypeType

def get_value() -> EvaluationTaskTypeType:
    return "Classification"
```

```python
# EvaluationTaskTypeType definition

EvaluationTaskTypeType = Literal[
    "Classification",
    "Custom",
    "Generation",
    "QuestionAndAnswer",
    "Summarization",
]
```
## ExternalSourceTypeType

```python
# ExternalSourceTypeType usage example

from types_aiobotocore_bedrock.literals import ExternalSourceTypeType

def get_value() -> ExternalSourceTypeType:
    return "BYTE_CONTENT"
```

```python
# ExternalSourceTypeType definition

ExternalSourceTypeType = Literal[
    "BYTE_CONTENT",
    "S3",
]
```
## FineTuningJobStatusType

```python
# FineTuningJobStatusType usage example

from types_aiobotocore_bedrock.literals import FineTuningJobStatusType

def get_value() -> FineTuningJobStatusType:
    return "Completed"
```

```python
# FineTuningJobStatusType definition

FineTuningJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## FoundationModelLifecycleStatusType

```python
# FoundationModelLifecycleStatusType usage example

from types_aiobotocore_bedrock.literals import FoundationModelLifecycleStatusType

def get_value() -> FoundationModelLifecycleStatusType:
    return "ACTIVE"
```

```python
# FoundationModelLifecycleStatusType definition

FoundationModelLifecycleStatusType = Literal[
    "ACTIVE",
    "LEGACY",
]
```
## GuardrailContentFilterTypeType

```python
# GuardrailContentFilterTypeType usage example

from types_aiobotocore_bedrock.literals import GuardrailContentFilterTypeType

def get_value() -> GuardrailContentFilterTypeType:
    return "HATE"
```

```python
# GuardrailContentFilterTypeType definition

GuardrailContentFilterTypeType = Literal[
    "HATE",
    "INSULTS",
    "MISCONDUCT",
    "PROMPT_ATTACK",
    "SEXUAL",
    "VIOLENCE",
]
```
## GuardrailContextualGroundingFilterTypeType

```python
# GuardrailContextualGroundingFilterTypeType usage example

from types_aiobotocore_bedrock.literals import GuardrailContextualGroundingFilterTypeType

def get_value() -> GuardrailContextualGroundingFilterTypeType:
    return "GROUNDING"
```

```python
# GuardrailContextualGroundingFilterTypeType definition

GuardrailContextualGroundingFilterTypeType = Literal[
    "GROUNDING",
    "RELEVANCE",
]
```
## GuardrailFilterStrengthType

```python
# GuardrailFilterStrengthType usage example

from types_aiobotocore_bedrock.literals import GuardrailFilterStrengthType

def get_value() -> GuardrailFilterStrengthType:
    return "HIGH"
```

```python
# GuardrailFilterStrengthType definition

GuardrailFilterStrengthType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
    "NONE",
]
```
## GuardrailManagedWordsTypeType

```python
# GuardrailManagedWordsTypeType usage example

from types_aiobotocore_bedrock.literals import GuardrailManagedWordsTypeType

def get_value() -> GuardrailManagedWordsTypeType:
    return "PROFANITY"
```

```python
# GuardrailManagedWordsTypeType definition

GuardrailManagedWordsTypeType = Literal[
    "PROFANITY",
]
```
## GuardrailModalityType

```python
# GuardrailModalityType usage example

from types_aiobotocore_bedrock.literals import GuardrailModalityType

def get_value() -> GuardrailModalityType:
    return "IMAGE"
```

```python
# GuardrailModalityType definition

GuardrailModalityType = Literal[
    "IMAGE",
    "TEXT",
]
```
## GuardrailPiiEntityTypeType

```python
# GuardrailPiiEntityTypeType usage example

from types_aiobotocore_bedrock.literals import GuardrailPiiEntityTypeType

def get_value() -> GuardrailPiiEntityTypeType:
    return "ADDRESS"
```

```python
# GuardrailPiiEntityTypeType definition

GuardrailPiiEntityTypeType = Literal[
    "ADDRESS",
    "AGE",
    "AWS_ACCESS_KEY",
    "AWS_SECRET_KEY",
    "CA_HEALTH_NUMBER",
    "CA_SOCIAL_INSURANCE_NUMBER",
    "CREDIT_DEBIT_CARD_CVV",
    "CREDIT_DEBIT_CARD_EXPIRY",
    "CREDIT_DEBIT_CARD_NUMBER",
    "DRIVER_ID",
    "EMAIL",
    "INTERNATIONAL_BANK_ACCOUNT_NUMBER",
    "IP_ADDRESS",
    "LICENSE_PLATE",
    "MAC_ADDRESS",
    "NAME",
    "PASSWORD",
    "PHONE",
    "PIN",
    "SWIFT_CODE",
    "UK_NATIONAL_HEALTH_SERVICE_NUMBER",
    "UK_NATIONAL_INSURANCE_NUMBER",
    "UK_UNIQUE_TAXPAYER_REFERENCE_NUMBER",
    "URL",
    "US_BANK_ACCOUNT_NUMBER",
    "US_BANK_ROUTING_NUMBER",
    "US_INDIVIDUAL_TAX_IDENTIFICATION_NUMBER",
    "US_PASSPORT_NUMBER",
    "US_SOCIAL_SECURITY_NUMBER",
    "USERNAME",
    "VEHICLE_IDENTIFICATION_NUMBER",
]
```
## GuardrailSensitiveInformationActionType

```python
# GuardrailSensitiveInformationActionType usage example

from types_aiobotocore_bedrock.literals import GuardrailSensitiveInformationActionType

def get_value() -> GuardrailSensitiveInformationActionType:
    return "ANONYMIZE"
```

```python
# GuardrailSensitiveInformationActionType definition

GuardrailSensitiveInformationActionType = Literal[
    "ANONYMIZE",
    "BLOCK",
]
```
## GuardrailStatusType

```python
# GuardrailStatusType usage example

from types_aiobotocore_bedrock.literals import GuardrailStatusType

def get_value() -> GuardrailStatusType:
    return "CREATING"
```

```python
# GuardrailStatusType definition

GuardrailStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "READY",
    "UPDATING",
    "VERSIONING",
]
```
## GuardrailTopicTypeType

```python
# GuardrailTopicTypeType usage example

from types_aiobotocore_bedrock.literals import GuardrailTopicTypeType

def get_value() -> GuardrailTopicTypeType:
    return "DENY"
```

```python
# GuardrailTopicTypeType definition

GuardrailTopicTypeType = Literal[
    "DENY",
]
```
## InferenceProfileStatusType

```python
# InferenceProfileStatusType usage example

from types_aiobotocore_bedrock.literals import InferenceProfileStatusType

def get_value() -> InferenceProfileStatusType:
    return "ACTIVE"
```

```python
# InferenceProfileStatusType definition

InferenceProfileStatusType = Literal[
    "ACTIVE",
]
```
## InferenceProfileTypeType

```python
# InferenceProfileTypeType usage example

from types_aiobotocore_bedrock.literals import InferenceProfileTypeType

def get_value() -> InferenceProfileTypeType:
    return "APPLICATION"
```

```python
# InferenceProfileTypeType definition

InferenceProfileTypeType = Literal[
    "APPLICATION",
    "SYSTEM_DEFINED",
]
```
## InferenceTypeType

```python
# InferenceTypeType usage example

from types_aiobotocore_bedrock.literals import InferenceTypeType

def get_value() -> InferenceTypeType:
    return "ON_DEMAND"
```

```python
# InferenceTypeType definition

InferenceTypeType = Literal[
    "ON_DEMAND",
    "PROVISIONED",
]
```
## ListCustomModelsPaginatorName

```python
# ListCustomModelsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListCustomModelsPaginatorName

def get_value() -> ListCustomModelsPaginatorName:
    return "list_custom_models"
```

```python
# ListCustomModelsPaginatorName definition

ListCustomModelsPaginatorName = Literal[
    "list_custom_models",
]
```
## ListEvaluationJobsPaginatorName

```python
# ListEvaluationJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListEvaluationJobsPaginatorName

def get_value() -> ListEvaluationJobsPaginatorName:
    return "list_evaluation_jobs"
```

```python
# ListEvaluationJobsPaginatorName definition

ListEvaluationJobsPaginatorName = Literal[
    "list_evaluation_jobs",
]
```
## ListGuardrailsPaginatorName

```python
# ListGuardrailsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListGuardrailsPaginatorName

def get_value() -> ListGuardrailsPaginatorName:
    return "list_guardrails"
```

```python
# ListGuardrailsPaginatorName definition

ListGuardrailsPaginatorName = Literal[
    "list_guardrails",
]
```
## ListImportedModelsPaginatorName

```python
# ListImportedModelsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListImportedModelsPaginatorName

def get_value() -> ListImportedModelsPaginatorName:
    return "list_imported_models"
```

```python
# ListImportedModelsPaginatorName definition

ListImportedModelsPaginatorName = Literal[
    "list_imported_models",
]
```
## ListInferenceProfilesPaginatorName

```python
# ListInferenceProfilesPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListInferenceProfilesPaginatorName

def get_value() -> ListInferenceProfilesPaginatorName:
    return "list_inference_profiles"
```

```python
# ListInferenceProfilesPaginatorName definition

ListInferenceProfilesPaginatorName = Literal[
    "list_inference_profiles",
]
```
## ListMarketplaceModelEndpointsPaginatorName

```python
# ListMarketplaceModelEndpointsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListMarketplaceModelEndpointsPaginatorName

def get_value() -> ListMarketplaceModelEndpointsPaginatorName:
    return "list_marketplace_model_endpoints"
```

```python
# ListMarketplaceModelEndpointsPaginatorName definition

ListMarketplaceModelEndpointsPaginatorName = Literal[
    "list_marketplace_model_endpoints",
]
```
## ListModelCopyJobsPaginatorName

```python
# ListModelCopyJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListModelCopyJobsPaginatorName

def get_value() -> ListModelCopyJobsPaginatorName:
    return "list_model_copy_jobs"
```

```python
# ListModelCopyJobsPaginatorName definition

ListModelCopyJobsPaginatorName = Literal[
    "list_model_copy_jobs",
]
```
## ListModelCustomizationJobsPaginatorName

```python
# ListModelCustomizationJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListModelCustomizationJobsPaginatorName

def get_value() -> ListModelCustomizationJobsPaginatorName:
    return "list_model_customization_jobs"
```

```python
# ListModelCustomizationJobsPaginatorName definition

ListModelCustomizationJobsPaginatorName = Literal[
    "list_model_customization_jobs",
]
```
## ListModelImportJobsPaginatorName

```python
# ListModelImportJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListModelImportJobsPaginatorName

def get_value() -> ListModelImportJobsPaginatorName:
    return "list_model_import_jobs"
```

```python
# ListModelImportJobsPaginatorName definition

ListModelImportJobsPaginatorName = Literal[
    "list_model_import_jobs",
]
```
## ListModelInvocationJobsPaginatorName

```python
# ListModelInvocationJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListModelInvocationJobsPaginatorName

def get_value() -> ListModelInvocationJobsPaginatorName:
    return "list_model_invocation_jobs"
```

```python
# ListModelInvocationJobsPaginatorName definition

ListModelInvocationJobsPaginatorName = Literal[
    "list_model_invocation_jobs",
]
```
## ListPromptRoutersPaginatorName

```python
# ListPromptRoutersPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListPromptRoutersPaginatorName

def get_value() -> ListPromptRoutersPaginatorName:
    return "list_prompt_routers"
```

```python
# ListPromptRoutersPaginatorName definition

ListPromptRoutersPaginatorName = Literal[
    "list_prompt_routers",
]
```
## ListProvisionedModelThroughputsPaginatorName

```python
# ListProvisionedModelThroughputsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListProvisionedModelThroughputsPaginatorName

def get_value() -> ListProvisionedModelThroughputsPaginatorName:
    return "list_provisioned_model_throughputs"
```

```python
# ListProvisionedModelThroughputsPaginatorName definition

ListProvisionedModelThroughputsPaginatorName = Literal[
    "list_provisioned_model_throughputs",
]
```
## ModelCopyJobStatusType

```python
# ModelCopyJobStatusType usage example

from types_aiobotocore_bedrock.literals import ModelCopyJobStatusType

def get_value() -> ModelCopyJobStatusType:
    return "Completed"
```

```python
# ModelCopyJobStatusType definition

ModelCopyJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
]
```
## ModelCustomizationJobStatusType

```python
# ModelCustomizationJobStatusType usage example

from types_aiobotocore_bedrock.literals import ModelCustomizationJobStatusType

def get_value() -> ModelCustomizationJobStatusType:
    return "Completed"
```

```python
# ModelCustomizationJobStatusType definition

ModelCustomizationJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## ModelCustomizationType

```python
# ModelCustomizationType usage example

from types_aiobotocore_bedrock.literals import ModelCustomizationType

def get_value() -> ModelCustomizationType:
    return "CONTINUED_PRE_TRAINING"
```

```python
# ModelCustomizationType definition

ModelCustomizationType = Literal[
    "CONTINUED_PRE_TRAINING",
    "DISTILLATION",
    "FINE_TUNING",
]
```
## ModelImportJobStatusType

```python
# ModelImportJobStatusType usage example

from types_aiobotocore_bedrock.literals import ModelImportJobStatusType

def get_value() -> ModelImportJobStatusType:
    return "Completed"
```

```python
# ModelImportJobStatusType definition

ModelImportJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
]
```
## ModelInvocationJobStatusType

```python
# ModelInvocationJobStatusType usage example

from types_aiobotocore_bedrock.literals import ModelInvocationJobStatusType

def get_value() -> ModelInvocationJobStatusType:
    return "Completed"
```

```python
# ModelInvocationJobStatusType definition

ModelInvocationJobStatusType = Literal[
    "Completed",
    "Expired",
    "Failed",
    "InProgress",
    "PartiallyCompleted",
    "Scheduled",
    "Stopped",
    "Stopping",
    "Submitted",
    "Validating",
]
```
## ModelModalityType

```python
# ModelModalityType usage example

from types_aiobotocore_bedrock.literals import ModelModalityType

def get_value() -> ModelModalityType:
    return "EMBEDDING"
```

```python
# ModelModalityType definition

ModelModalityType = Literal[
    "EMBEDDING",
    "IMAGE",
    "TEXT",
]
```
## PerformanceConfigLatencyType

```python
# PerformanceConfigLatencyType usage example

from types_aiobotocore_bedrock.literals import PerformanceConfigLatencyType

def get_value() -> PerformanceConfigLatencyType:
    return "optimized"
```

```python
# PerformanceConfigLatencyType definition

PerformanceConfigLatencyType = Literal[
    "optimized",
    "standard",
]
```
## PromptRouterStatusType

```python
# PromptRouterStatusType usage example

from types_aiobotocore_bedrock.literals import PromptRouterStatusType

def get_value() -> PromptRouterStatusType:
    return "AVAILABLE"
```

```python
# PromptRouterStatusType definition

PromptRouterStatusType = Literal[
    "AVAILABLE",
]
```
## PromptRouterTypeType

```python
# PromptRouterTypeType usage example

from types_aiobotocore_bedrock.literals import PromptRouterTypeType

def get_value() -> PromptRouterTypeType:
    return "custom"
```

```python
# PromptRouterTypeType definition

PromptRouterTypeType = Literal[
    "custom",
    "default",
]
```
## ProvisionedModelStatusType

```python
# ProvisionedModelStatusType usage example

from types_aiobotocore_bedrock.literals import ProvisionedModelStatusType

def get_value() -> ProvisionedModelStatusType:
    return "Creating"
```

```python
# ProvisionedModelStatusType definition

ProvisionedModelStatusType = Literal[
    "Creating",
    "Failed",
    "InService",
    "Updating",
]
```
## QueryTransformationTypeType

```python
# QueryTransformationTypeType usage example

from types_aiobotocore_bedrock.literals import QueryTransformationTypeType

def get_value() -> QueryTransformationTypeType:
    return "QUERY_DECOMPOSITION"
```

```python
# QueryTransformationTypeType definition

QueryTransformationTypeType = Literal[
    "QUERY_DECOMPOSITION",
]
```
## RetrieveAndGenerateTypeType

```python
# RetrieveAndGenerateTypeType usage example

from types_aiobotocore_bedrock.literals import RetrieveAndGenerateTypeType

def get_value() -> RetrieveAndGenerateTypeType:
    return "EXTERNAL_SOURCES"
```

```python
# RetrieveAndGenerateTypeType definition

RetrieveAndGenerateTypeType = Literal[
    "EXTERNAL_SOURCES",
    "KNOWLEDGE_BASE",
]
```
## S3InputFormatType

```python
# S3InputFormatType usage example

from types_aiobotocore_bedrock.literals import S3InputFormatType

def get_value() -> S3InputFormatType:
    return "JSONL"
```

```python
# S3InputFormatType definition

S3InputFormatType = Literal[
    "JSONL",
]
```
## SearchTypeType

```python
# SearchTypeType usage example

from types_aiobotocore_bedrock.literals import SearchTypeType

def get_value() -> SearchTypeType:
    return "HYBRID"
```

```python
# SearchTypeType definition

SearchTypeType = Literal[
    "HYBRID",
    "SEMANTIC",
]
```
## SortByProvisionedModelsType

```python
# SortByProvisionedModelsType usage example

from types_aiobotocore_bedrock.literals import SortByProvisionedModelsType

def get_value() -> SortByProvisionedModelsType:
    return "CreationTime"
```

```python
# SortByProvisionedModelsType definition

SortByProvisionedModelsType = Literal[
    "CreationTime",
]
```
## SortJobsByType

```python
# SortJobsByType usage example

from types_aiobotocore_bedrock.literals import SortJobsByType

def get_value() -> SortJobsByType:
    return "CreationTime"
```

```python
# SortJobsByType definition

SortJobsByType = Literal[
    "CreationTime",
]
```
## SortModelsByType

```python
# SortModelsByType usage example

from types_aiobotocore_bedrock.literals import SortModelsByType

def get_value() -> SortModelsByType:
    return "CreationTime"
```

```python
# SortModelsByType definition

SortModelsByType = Literal[
    "CreationTime",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_bedrock.literals import SortOrderType

def get_value() -> SortOrderType:
    return "Ascending"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "Ascending",
    "Descending",
]
```
## StatusType

```python
# StatusType usage example

from types_aiobotocore_bedrock.literals import StatusType

def get_value() -> StatusType:
    return "INCOMPATIBLE_ENDPOINT"
```

```python
# StatusType definition

StatusType = Literal[
    "INCOMPATIBLE_ENDPOINT",
    "REGISTERED",
]
```
## BedrockServiceName

```python
# BedrockServiceName usage example

from types_aiobotocore_bedrock.literals import BedrockServiceName

def get_value() -> BedrockServiceName:
    return "bedrock"
```

```python
# BedrockServiceName definition

BedrockServiceName = Literal[
    "bedrock",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_bedrock.literals import ServiceName

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

from types_aiobotocore_bedrock.literals import ResourceServiceName

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

from types_aiobotocore_bedrock.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_custom_models"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_custom_models",
    "list_evaluation_jobs",
    "list_guardrails",
    "list_imported_models",
    "list_inference_profiles",
    "list_marketplace_model_endpoints",
    "list_model_copy_jobs",
    "list_model_customization_jobs",
    "list_model_import_jobs",
    "list_model_invocation_jobs",
    "list_prompt_routers",
    "list_provisioned_model_throughputs",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_bedrock.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
