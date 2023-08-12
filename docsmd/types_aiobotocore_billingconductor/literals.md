# Literals

> [Index](../README.md) > [BillingConductor](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
    type annotations stubs module [types-aiobotocore-billingconductor](https://pypi.org/project/types-aiobotocore-billingconductor/).

## AssociateResourceErrorReasonType

```python
# AssociateResourceErrorReasonType usage example

from types_aiobotocore_billingconductor.literals import AssociateResourceErrorReasonType

def get_value() -> AssociateResourceErrorReasonType:
    return "ILLEGAL_CUSTOMLINEITEM"
```

```python
# AssociateResourceErrorReasonType definition

AssociateResourceErrorReasonType = Literal[
    "ILLEGAL_CUSTOMLINEITEM",
    "INTERNAL_SERVER_EXCEPTION",
    "INVALID_ARN",
    "INVALID_BILLING_PERIOD_RANGE",
    "SERVICE_LIMIT_EXCEEDED",
]
```
## BillingGroupStatusType

```python
# BillingGroupStatusType usage example

from types_aiobotocore_billingconductor.literals import BillingGroupStatusType

def get_value() -> BillingGroupStatusType:
    return "ACTIVE"
```

```python
# BillingGroupStatusType definition

BillingGroupStatusType = Literal[
    "ACTIVE",
    "PRIMARY_ACCOUNT_MISSING",
]
```
## CurrencyCodeType

```python
# CurrencyCodeType usage example

from types_aiobotocore_billingconductor.literals import CurrencyCodeType

def get_value() -> CurrencyCodeType:
    return "CNY"
```

```python
# CurrencyCodeType definition

CurrencyCodeType = Literal[
    "CNY",
    "USD",
]
```
## CustomLineItemRelationshipType

```python
# CustomLineItemRelationshipType usage example

from types_aiobotocore_billingconductor.literals import CustomLineItemRelationshipType

def get_value() -> CustomLineItemRelationshipType:
    return "CHILD"
```

```python
# CustomLineItemRelationshipType definition

CustomLineItemRelationshipType = Literal[
    "CHILD",
    "PARENT",
]
```
## CustomLineItemTypeType

```python
# CustomLineItemTypeType usage example

from types_aiobotocore_billingconductor.literals import CustomLineItemTypeType

def get_value() -> CustomLineItemTypeType:
    return "CREDIT"
```

```python
# CustomLineItemTypeType definition

CustomLineItemTypeType = Literal[
    "CREDIT",
    "FEE",
]
```
## ListAccountAssociationsPaginatorName

```python
# ListAccountAssociationsPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListAccountAssociationsPaginatorName

def get_value() -> ListAccountAssociationsPaginatorName:
    return "list_account_associations"
```

```python
# ListAccountAssociationsPaginatorName definition

ListAccountAssociationsPaginatorName = Literal[
    "list_account_associations",
]
```
## ListBillingGroupCostReportsPaginatorName

```python
# ListBillingGroupCostReportsPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListBillingGroupCostReportsPaginatorName

def get_value() -> ListBillingGroupCostReportsPaginatorName:
    return "list_billing_group_cost_reports"
```

```python
# ListBillingGroupCostReportsPaginatorName definition

ListBillingGroupCostReportsPaginatorName = Literal[
    "list_billing_group_cost_reports",
]
```
## ListBillingGroupsPaginatorName

```python
# ListBillingGroupsPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListBillingGroupsPaginatorName

def get_value() -> ListBillingGroupsPaginatorName:
    return "list_billing_groups"
```

```python
# ListBillingGroupsPaginatorName definition

ListBillingGroupsPaginatorName = Literal[
    "list_billing_groups",
]
```
## ListCustomLineItemVersionsPaginatorName

```python
# ListCustomLineItemVersionsPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListCustomLineItemVersionsPaginatorName

def get_value() -> ListCustomLineItemVersionsPaginatorName:
    return "list_custom_line_item_versions"
```

```python
# ListCustomLineItemVersionsPaginatorName definition

ListCustomLineItemVersionsPaginatorName = Literal[
    "list_custom_line_item_versions",
]
```
## ListCustomLineItemsPaginatorName

```python
# ListCustomLineItemsPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListCustomLineItemsPaginatorName

def get_value() -> ListCustomLineItemsPaginatorName:
    return "list_custom_line_items"
```

```python
# ListCustomLineItemsPaginatorName definition

ListCustomLineItemsPaginatorName = Literal[
    "list_custom_line_items",
]
```
## ListPricingPlansAssociatedWithPricingRulePaginatorName

```python
# ListPricingPlansAssociatedWithPricingRulePaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListPricingPlansAssociatedWithPricingRulePaginatorName

def get_value() -> ListPricingPlansAssociatedWithPricingRulePaginatorName:
    return "list_pricing_plans_associated_with_pricing_rule"
```

```python
# ListPricingPlansAssociatedWithPricingRulePaginatorName definition

ListPricingPlansAssociatedWithPricingRulePaginatorName = Literal[
    "list_pricing_plans_associated_with_pricing_rule",
]
```
## ListPricingPlansPaginatorName

```python
# ListPricingPlansPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListPricingPlansPaginatorName

def get_value() -> ListPricingPlansPaginatorName:
    return "list_pricing_plans"
```

```python
# ListPricingPlansPaginatorName definition

ListPricingPlansPaginatorName = Literal[
    "list_pricing_plans",
]
```
## ListPricingRulesAssociatedToPricingPlanPaginatorName

```python
# ListPricingRulesAssociatedToPricingPlanPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListPricingRulesAssociatedToPricingPlanPaginatorName

def get_value() -> ListPricingRulesAssociatedToPricingPlanPaginatorName:
    return "list_pricing_rules_associated_to_pricing_plan"
```

```python
# ListPricingRulesAssociatedToPricingPlanPaginatorName definition

ListPricingRulesAssociatedToPricingPlanPaginatorName = Literal[
    "list_pricing_rules_associated_to_pricing_plan",
]
```
## ListPricingRulesPaginatorName

```python
# ListPricingRulesPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListPricingRulesPaginatorName

def get_value() -> ListPricingRulesPaginatorName:
    return "list_pricing_rules"
```

```python
# ListPricingRulesPaginatorName definition

ListPricingRulesPaginatorName = Literal[
    "list_pricing_rules",
]
```
## ListResourcesAssociatedToCustomLineItemPaginatorName

```python
# ListResourcesAssociatedToCustomLineItemPaginatorName usage example

from types_aiobotocore_billingconductor.literals import ListResourcesAssociatedToCustomLineItemPaginatorName

def get_value() -> ListResourcesAssociatedToCustomLineItemPaginatorName:
    return "list_resources_associated_to_custom_line_item"
```

```python
# ListResourcesAssociatedToCustomLineItemPaginatorName definition

ListResourcesAssociatedToCustomLineItemPaginatorName = Literal[
    "list_resources_associated_to_custom_line_item",
]
```
## PricingRuleScopeType

```python
# PricingRuleScopeType usage example

from types_aiobotocore_billingconductor.literals import PricingRuleScopeType

def get_value() -> PricingRuleScopeType:
    return "BILLING_ENTITY"
```

```python
# PricingRuleScopeType definition

PricingRuleScopeType = Literal[
    "BILLING_ENTITY",
    "GLOBAL",
    "SERVICE",
    "SKU",
]
```
## PricingRuleTypeType

```python
# PricingRuleTypeType usage example

from types_aiobotocore_billingconductor.literals import PricingRuleTypeType

def get_value() -> PricingRuleTypeType:
    return "DISCOUNT"
```

```python
# PricingRuleTypeType definition

PricingRuleTypeType = Literal[
    "DISCOUNT",
    "MARKUP",
    "TIERING",
]
```
## BillingConductorServiceName

```python
# BillingConductorServiceName usage example

from types_aiobotocore_billingconductor.literals import BillingConductorServiceName

def get_value() -> BillingConductorServiceName:
    return "billingconductor"
```

```python
# BillingConductorServiceName definition

BillingConductorServiceName = Literal[
    "billingconductor",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_billingconductor.literals import ServiceName

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

from types_aiobotocore_billingconductor.literals import ResourceServiceName

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

from types_aiobotocore_billingconductor.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_account_associations"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_account_associations",
    "list_billing_group_cost_reports",
    "list_billing_groups",
    "list_custom_line_item_versions",
    "list_custom_line_items",
    "list_pricing_plans",
    "list_pricing_plans_associated_with_pricing_rule",
    "list_pricing_rules",
    "list_pricing_rules_associated_to_pricing_plan",
    "list_resources_associated_to_custom_line_item",
]
```
