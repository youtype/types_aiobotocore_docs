# Literals

> [Index](../README.md) > [CloudWatchApplicationSignals](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals)
    type annotations stubs module [types-aiobotocore-application-signals](https://pypi.org/project/types-aiobotocore-application-signals/).

## ChangeEventTypeType

```python
# ChangeEventTypeType usage example
from types_aiobotocore_application_signals.literals import ChangeEventTypeType

def get_value() -> ChangeEventTypeType:
    return "CONFIGURATION"
```

```python
# ChangeEventTypeType definition
ChangeEventTypeType = Literal[
    "CONFIGURATION",
    "DEPLOYMENT",
]
```
## ConnectionTypeType

```python
# ConnectionTypeType usage example
from types_aiobotocore_application_signals.literals import ConnectionTypeType

def get_value() -> ConnectionTypeType:
    return "DIRECT"
```

```python
# ConnectionTypeType definition
ConnectionTypeType = Literal[
    "DIRECT",
    "INDIRECT",
]
```
## DetailLevelType

```python
# DetailLevelType usage example
from types_aiobotocore_application_signals.literals import DetailLevelType

def get_value() -> DetailLevelType:
    return "BRIEF"
```

```python
# DetailLevelType definition
DetailLevelType = Literal[
    "BRIEF",
    "DETAILED",
]
```
## DurationUnitType

```python
# DurationUnitType usage example
from types_aiobotocore_application_signals.literals import DurationUnitType

def get_value() -> DurationUnitType:
    return "DAY"
```

```python
# DurationUnitType definition
DurationUnitType = Literal[
    "DAY",
    "HOUR",
    "MINUTE",
    "MONTH",
]
```
## EvaluationTypeType

```python
# EvaluationTypeType usage example
from types_aiobotocore_application_signals.literals import EvaluationTypeType

def get_value() -> EvaluationTypeType:
    return "PeriodBased"
```

```python
# EvaluationTypeType definition
EvaluationTypeType = Literal[
    "PeriodBased",
    "RequestBased",
]
```
## ListEntityEventsPaginatorName

```python
# ListEntityEventsPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListEntityEventsPaginatorName

def get_value() -> ListEntityEventsPaginatorName:
    return "list_entity_events"
```

```python
# ListEntityEventsPaginatorName definition
ListEntityEventsPaginatorName = Literal[
    "list_entity_events",
]
```
## ListServiceDependenciesPaginatorName

```python
# ListServiceDependenciesPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceDependenciesPaginatorName

def get_value() -> ListServiceDependenciesPaginatorName:
    return "list_service_dependencies"
```

```python
# ListServiceDependenciesPaginatorName definition
ListServiceDependenciesPaginatorName = Literal[
    "list_service_dependencies",
]
```
## ListServiceDependentsPaginatorName

```python
# ListServiceDependentsPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceDependentsPaginatorName

def get_value() -> ListServiceDependentsPaginatorName:
    return "list_service_dependents"
```

```python
# ListServiceDependentsPaginatorName definition
ListServiceDependentsPaginatorName = Literal[
    "list_service_dependents",
]
```
## ListServiceLevelObjectiveExclusionWindowsPaginatorName

```python
# ListServiceLevelObjectiveExclusionWindowsPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceLevelObjectiveExclusionWindowsPaginatorName

def get_value() -> ListServiceLevelObjectiveExclusionWindowsPaginatorName:
    return "list_service_level_objective_exclusion_windows"
```

```python
# ListServiceLevelObjectiveExclusionWindowsPaginatorName definition
ListServiceLevelObjectiveExclusionWindowsPaginatorName = Literal[
    "list_service_level_objective_exclusion_windows",
]
```
## ListServiceLevelObjectivesPaginatorName

```python
# ListServiceLevelObjectivesPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceLevelObjectivesPaginatorName

def get_value() -> ListServiceLevelObjectivesPaginatorName:
    return "list_service_level_objectives"
```

```python
# ListServiceLevelObjectivesPaginatorName definition
ListServiceLevelObjectivesPaginatorName = Literal[
    "list_service_level_objectives",
]
```
## ListServiceOperationsPaginatorName

```python
# ListServiceOperationsPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceOperationsPaginatorName

def get_value() -> ListServiceOperationsPaginatorName:
    return "list_service_operations"
```

```python
# ListServiceOperationsPaginatorName definition
ListServiceOperationsPaginatorName = Literal[
    "list_service_operations",
]
```
## ListServiceStatesPaginatorName

```python
# ListServiceStatesPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServiceStatesPaginatorName

def get_value() -> ListServiceStatesPaginatorName:
    return "list_service_states"
```

```python
# ListServiceStatesPaginatorName definition
ListServiceStatesPaginatorName = Literal[
    "list_service_states",
]
```
## ListServicesPaginatorName

```python
# ListServicesPaginatorName usage example
from types_aiobotocore_application_signals.literals import ListServicesPaginatorName

def get_value() -> ListServicesPaginatorName:
    return "list_services"
```

```python
# ListServicesPaginatorName definition
ListServicesPaginatorName = Literal[
    "list_services",
]
```
## MetricSourceTypeType

```python
# MetricSourceTypeType usage example
from types_aiobotocore_application_signals.literals import MetricSourceTypeType

def get_value() -> MetricSourceTypeType:
    return "CloudWatchMetric"
```

```python
# MetricSourceTypeType definition
MetricSourceTypeType = Literal[
    "CloudWatchMetric",
    "ServiceDependency",
    "ServiceOperation",
]
```
## ServiceLevelIndicatorComparisonOperatorType

```python
# ServiceLevelIndicatorComparisonOperatorType usage example
from types_aiobotocore_application_signals.literals import ServiceLevelIndicatorComparisonOperatorType

def get_value() -> ServiceLevelIndicatorComparisonOperatorType:
    return "GreaterThan"
```

```python
# ServiceLevelIndicatorComparisonOperatorType definition
ServiceLevelIndicatorComparisonOperatorType = Literal[
    "GreaterThan",
    "GreaterThanOrEqualTo",
    "LessThan",
    "LessThanOrEqualTo",
]
```
## ServiceLevelIndicatorMetricTypeType

```python
# ServiceLevelIndicatorMetricTypeType usage example
from types_aiobotocore_application_signals.literals import ServiceLevelIndicatorMetricTypeType

def get_value() -> ServiceLevelIndicatorMetricTypeType:
    return "AVAILABILITY"
```

```python
# ServiceLevelIndicatorMetricTypeType definition
ServiceLevelIndicatorMetricTypeType = Literal[
    "AVAILABILITY",
    "LATENCY",
]
```
## ServiceLevelObjectiveBudgetStatusType

```python
# ServiceLevelObjectiveBudgetStatusType usage example
from types_aiobotocore_application_signals.literals import ServiceLevelObjectiveBudgetStatusType

def get_value() -> ServiceLevelObjectiveBudgetStatusType:
    return "BREACHED"
```

```python
# ServiceLevelObjectiveBudgetStatusType definition
ServiceLevelObjectiveBudgetStatusType = Literal[
    "BREACHED",
    "INSUFFICIENT_DATA",
    "OK",
    "WARNING",
]
```
## SeverityType

```python
# SeverityType usage example
from types_aiobotocore_application_signals.literals import SeverityType

def get_value() -> SeverityType:
    return "CRITICAL"
```

```python
# SeverityType definition
SeverityType = Literal[
    "CRITICAL",
    "HIGH",
    "LOW",
    "MEDIUM",
    "NONE",
]
```
## StandardUnitType

```python
# StandardUnitType usage example
from types_aiobotocore_application_signals.literals import StandardUnitType

def get_value() -> StandardUnitType:
    return "Bits"
```

```python
# StandardUnitType definition
StandardUnitType = Literal[
    "Bits",
    "Bits/Second",
    "Bytes",
    "Bytes/Second",
    "Count",
    "Count/Second",
    "Gigabits",
    "Gigabits/Second",
    "Gigabytes",
    "Gigabytes/Second",
    "Kilobits",
    "Kilobits/Second",
    "Kilobytes",
    "Kilobytes/Second",
    "Megabits",
    "Megabits/Second",
    "Megabytes",
    "Megabytes/Second",
    "Microseconds",
    "Milliseconds",
    "None",
    "Percent",
    "Seconds",
    "Terabits",
    "Terabits/Second",
    "Terabytes",
    "Terabytes/Second",
]
```
## CloudWatchApplicationSignalsServiceName

```python
# CloudWatchApplicationSignalsServiceName usage example
from types_aiobotocore_application_signals.literals import CloudWatchApplicationSignalsServiceName

def get_value() -> CloudWatchApplicationSignalsServiceName:
    return "application-signals"
```

```python
# CloudWatchApplicationSignalsServiceName definition
CloudWatchApplicationSignalsServiceName = Literal[
    "application-signals",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_application_signals.literals import ServiceName

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
from types_aiobotocore_application_signals.literals import ResourceServiceName

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
from types_aiobotocore_application_signals.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_entity_events"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_entity_events",
    "list_service_dependencies",
    "list_service_dependents",
    "list_service_level_objective_exclusion_windows",
    "list_service_level_objectives",
    "list_service_operations",
    "list_service_states",
    "list_services",
]
```
