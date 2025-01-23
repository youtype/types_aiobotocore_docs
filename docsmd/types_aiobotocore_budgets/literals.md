# Literals

> [Index](../README.md) > [Budgets](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## ActionStatusType

```python
# ActionStatusType usage example

from types_aiobotocore_budgets.literals import ActionStatusType

def get_value() -> ActionStatusType:
    return "EXECUTION_FAILURE"
```

```python
# ActionStatusType definition

ActionStatusType = Literal[
    "EXECUTION_FAILURE",
    "EXECUTION_IN_PROGRESS",
    "EXECUTION_SUCCESS",
    "PENDING",
    "RESET_FAILURE",
    "RESET_IN_PROGRESS",
    "REVERSE_FAILURE",
    "REVERSE_IN_PROGRESS",
    "REVERSE_SUCCESS",
    "STANDBY",
]
```
## ActionSubTypeType

```python
# ActionSubTypeType usage example

from types_aiobotocore_budgets.literals import ActionSubTypeType

def get_value() -> ActionSubTypeType:
    return "STOP_EC2_INSTANCES"
```

```python
# ActionSubTypeType definition

ActionSubTypeType = Literal[
    "STOP_EC2_INSTANCES",
    "STOP_RDS_INSTANCES",
]
```
## ActionTypeType

```python
# ActionTypeType usage example

from types_aiobotocore_budgets.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "APPLY_IAM_POLICY"
```

```python
# ActionTypeType definition

ActionTypeType = Literal[
    "APPLY_IAM_POLICY",
    "APPLY_SCP_POLICY",
    "RUN_SSM_DOCUMENTS",
]
```
## ApprovalModelType

```python
# ApprovalModelType usage example

from types_aiobotocore_budgets.literals import ApprovalModelType

def get_value() -> ApprovalModelType:
    return "AUTOMATIC"
```

```python
# ApprovalModelType definition

ApprovalModelType = Literal[
    "AUTOMATIC",
    "MANUAL",
]
```
## AutoAdjustTypeType

```python
# AutoAdjustTypeType usage example

from types_aiobotocore_budgets.literals import AutoAdjustTypeType

def get_value() -> AutoAdjustTypeType:
    return "FORECAST"
```

```python
# AutoAdjustTypeType definition

AutoAdjustTypeType = Literal[
    "FORECAST",
    "HISTORICAL",
]
```
## BudgetTypeType

```python
# BudgetTypeType usage example

from types_aiobotocore_budgets.literals import BudgetTypeType

def get_value() -> BudgetTypeType:
    return "COST"
```

```python
# BudgetTypeType definition

BudgetTypeType = Literal[
    "COST",
    "RI_COVERAGE",
    "RI_UTILIZATION",
    "SAVINGS_PLANS_COVERAGE",
    "SAVINGS_PLANS_UTILIZATION",
    "USAGE",
]
```
## ComparisonOperatorType

```python
# ComparisonOperatorType usage example

from types_aiobotocore_budgets.literals import ComparisonOperatorType

def get_value() -> ComparisonOperatorType:
    return "EQUAL_TO"
```

```python
# ComparisonOperatorType definition

ComparisonOperatorType = Literal[
    "EQUAL_TO",
    "GREATER_THAN",
    "LESS_THAN",
]
```
## DescribeBudgetActionHistoriesPaginatorName

```python
# DescribeBudgetActionHistoriesPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetActionHistoriesPaginatorName

def get_value() -> DescribeBudgetActionHistoriesPaginatorName:
    return "describe_budget_action_histories"
```

```python
# DescribeBudgetActionHistoriesPaginatorName definition

DescribeBudgetActionHistoriesPaginatorName = Literal[
    "describe_budget_action_histories",
]
```
## DescribeBudgetActionsForAccountPaginatorName

```python
# DescribeBudgetActionsForAccountPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetActionsForAccountPaginatorName

def get_value() -> DescribeBudgetActionsForAccountPaginatorName:
    return "describe_budget_actions_for_account"
```

```python
# DescribeBudgetActionsForAccountPaginatorName definition

DescribeBudgetActionsForAccountPaginatorName = Literal[
    "describe_budget_actions_for_account",
]
```
## DescribeBudgetActionsForBudgetPaginatorName

```python
# DescribeBudgetActionsForBudgetPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetActionsForBudgetPaginatorName

def get_value() -> DescribeBudgetActionsForBudgetPaginatorName:
    return "describe_budget_actions_for_budget"
```

```python
# DescribeBudgetActionsForBudgetPaginatorName definition

DescribeBudgetActionsForBudgetPaginatorName = Literal[
    "describe_budget_actions_for_budget",
]
```
## DescribeBudgetNotificationsForAccountPaginatorName

```python
# DescribeBudgetNotificationsForAccountPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetNotificationsForAccountPaginatorName

def get_value() -> DescribeBudgetNotificationsForAccountPaginatorName:
    return "describe_budget_notifications_for_account"
```

```python
# DescribeBudgetNotificationsForAccountPaginatorName definition

DescribeBudgetNotificationsForAccountPaginatorName = Literal[
    "describe_budget_notifications_for_account",
]
```
## DescribeBudgetPerformanceHistoryPaginatorName

```python
# DescribeBudgetPerformanceHistoryPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetPerformanceHistoryPaginatorName

def get_value() -> DescribeBudgetPerformanceHistoryPaginatorName:
    return "describe_budget_performance_history"
```

```python
# DescribeBudgetPerformanceHistoryPaginatorName definition

DescribeBudgetPerformanceHistoryPaginatorName = Literal[
    "describe_budget_performance_history",
]
```
## DescribeBudgetsPaginatorName

```python
# DescribeBudgetsPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeBudgetsPaginatorName

def get_value() -> DescribeBudgetsPaginatorName:
    return "describe_budgets"
```

```python
# DescribeBudgetsPaginatorName definition

DescribeBudgetsPaginatorName = Literal[
    "describe_budgets",
]
```
## DescribeNotificationsForBudgetPaginatorName

```python
# DescribeNotificationsForBudgetPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeNotificationsForBudgetPaginatorName

def get_value() -> DescribeNotificationsForBudgetPaginatorName:
    return "describe_notifications_for_budget"
```

```python
# DescribeNotificationsForBudgetPaginatorName definition

DescribeNotificationsForBudgetPaginatorName = Literal[
    "describe_notifications_for_budget",
]
```
## DescribeSubscribersForNotificationPaginatorName

```python
# DescribeSubscribersForNotificationPaginatorName usage example

from types_aiobotocore_budgets.literals import DescribeSubscribersForNotificationPaginatorName

def get_value() -> DescribeSubscribersForNotificationPaginatorName:
    return "describe_subscribers_for_notification"
```

```python
# DescribeSubscribersForNotificationPaginatorName definition

DescribeSubscribersForNotificationPaginatorName = Literal[
    "describe_subscribers_for_notification",
]
```
## EventTypeType

```python
# EventTypeType usage example

from types_aiobotocore_budgets.literals import EventTypeType

def get_value() -> EventTypeType:
    return "CREATE_ACTION"
```

```python
# EventTypeType definition

EventTypeType = Literal[
    "CREATE_ACTION",
    "DELETE_ACTION",
    "EXECUTE_ACTION",
    "SYSTEM",
    "UPDATE_ACTION",
]
```
## ExecutionTypeType

```python
# ExecutionTypeType usage example

from types_aiobotocore_budgets.literals import ExecutionTypeType

def get_value() -> ExecutionTypeType:
    return "APPROVE_BUDGET_ACTION"
```

```python
# ExecutionTypeType definition

ExecutionTypeType = Literal[
    "APPROVE_BUDGET_ACTION",
    "RESET_BUDGET_ACTION",
    "RETRY_BUDGET_ACTION",
    "REVERSE_BUDGET_ACTION",
]
```
## NotificationStateType

```python
# NotificationStateType usage example

from types_aiobotocore_budgets.literals import NotificationStateType

def get_value() -> NotificationStateType:
    return "ALARM"
```

```python
# NotificationStateType definition

NotificationStateType = Literal[
    "ALARM",
    "OK",
]
```
## NotificationTypeType

```python
# NotificationTypeType usage example

from types_aiobotocore_budgets.literals import NotificationTypeType

def get_value() -> NotificationTypeType:
    return "ACTUAL"
```

```python
# NotificationTypeType definition

NotificationTypeType = Literal[
    "ACTUAL",
    "FORECASTED",
]
```
## SubscriptionTypeType

```python
# SubscriptionTypeType usage example

from types_aiobotocore_budgets.literals import SubscriptionTypeType

def get_value() -> SubscriptionTypeType:
    return "EMAIL"
```

```python
# SubscriptionTypeType definition

SubscriptionTypeType = Literal[
    "EMAIL",
    "SNS",
]
```
## ThresholdTypeType

```python
# ThresholdTypeType usage example

from types_aiobotocore_budgets.literals import ThresholdTypeType

def get_value() -> ThresholdTypeType:
    return "ABSOLUTE_VALUE"
```

```python
# ThresholdTypeType definition

ThresholdTypeType = Literal[
    "ABSOLUTE_VALUE",
    "PERCENTAGE",
]
```
## TimeUnitType

```python
# TimeUnitType usage example

from types_aiobotocore_budgets.literals import TimeUnitType

def get_value() -> TimeUnitType:
    return "ANNUALLY"
```

```python
# TimeUnitType definition

TimeUnitType = Literal[
    "ANNUALLY",
    "DAILY",
    "MONTHLY",
    "QUARTERLY",
]
```
## BudgetsServiceName

```python
# BudgetsServiceName usage example

from types_aiobotocore_budgets.literals import BudgetsServiceName

def get_value() -> BudgetsServiceName:
    return "budgets"
```

```python
# BudgetsServiceName definition

BudgetsServiceName = Literal[
    "budgets",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_budgets.literals import ServiceName

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

from types_aiobotocore_budgets.literals import ResourceServiceName

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

from types_aiobotocore_budgets.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_budget_action_histories"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_budget_action_histories",
    "describe_budget_actions_for_account",
    "describe_budget_actions_for_budget",
    "describe_budget_notifications_for_account",
    "describe_budget_performance_history",
    "describe_budgets",
    "describe_notifications_for_budget",
    "describe_subscribers_for_notification",
]
```
