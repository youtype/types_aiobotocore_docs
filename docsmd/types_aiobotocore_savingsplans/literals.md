# Literals

> [Index](../README.md) > [SavingsPlans](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#savingsplans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## CurrencyCodeType

```python
# CurrencyCodeType usage example
from types_aiobotocore_savingsplans.literals import CurrencyCodeType

def get_value() -> CurrencyCodeType:
    return "CNY"
```

```python
# CurrencyCodeType definition
CurrencyCodeType = Literal[
    "CNY",
    "EUR",
    "USD",
]
```
## SavingsPlanOfferingFilterAttributeType

```python
# SavingsPlanOfferingFilterAttributeType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanOfferingFilterAttributeType

def get_value() -> SavingsPlanOfferingFilterAttributeType:
    return "instanceFamily"
```

```python
# SavingsPlanOfferingFilterAttributeType definition
SavingsPlanOfferingFilterAttributeType = Literal[
    "instanceFamily",
    "region",
]
```
## SavingsPlanOfferingPropertyKeyType

```python
# SavingsPlanOfferingPropertyKeyType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanOfferingPropertyKeyType

def get_value() -> SavingsPlanOfferingPropertyKeyType:
    return "instanceFamily"
```

```python
# SavingsPlanOfferingPropertyKeyType definition
SavingsPlanOfferingPropertyKeyType = Literal[
    "instanceFamily",
    "region",
]
```
## SavingsPlanPaymentOptionType

```python
# SavingsPlanPaymentOptionType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanPaymentOptionType

def get_value() -> SavingsPlanPaymentOptionType:
    return "All Upfront"
```

```python
# SavingsPlanPaymentOptionType definition
SavingsPlanPaymentOptionType = Literal[
    "All Upfront",
    "No Upfront",
    "Partial Upfront",
]
```
## SavingsPlanProductTypeType

```python
# SavingsPlanProductTypeType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanProductTypeType

def get_value() -> SavingsPlanProductTypeType:
    return "DMS"
```

```python
# SavingsPlanProductTypeType definition
SavingsPlanProductTypeType = Literal[
    "DMS",
    "DocDB",
    "DSQL",
    "DynamoDB",
    "EC2",
    "ElastiCache",
    "Fargate",
    "Keyspaces",
    "Lambda",
    "Neptune",
    "RDS",
    "SageMaker",
    "Timestream",
]
```
## SavingsPlanRateFilterAttributeType

```python
# SavingsPlanRateFilterAttributeType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanRateFilterAttributeType

def get_value() -> SavingsPlanRateFilterAttributeType:
    return "instanceFamily"
```

```python
# SavingsPlanRateFilterAttributeType definition
SavingsPlanRateFilterAttributeType = Literal[
    "instanceFamily",
    "instanceType",
    "productDescription",
    "productId",
    "region",
    "tenancy",
]
```
## SavingsPlanRateFilterNameType

```python
# SavingsPlanRateFilterNameType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanRateFilterNameType

def get_value() -> SavingsPlanRateFilterNameType:
    return "instanceType"
```

```python
# SavingsPlanRateFilterNameType definition
SavingsPlanRateFilterNameType = Literal[
    "instanceType",
    "operation",
    "productDescription",
    "productType",
    "region",
    "serviceCode",
    "tenancy",
    "usageType",
]
```
## SavingsPlanRatePropertyKeyType

```python
# SavingsPlanRatePropertyKeyType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanRatePropertyKeyType

def get_value() -> SavingsPlanRatePropertyKeyType:
    return "instanceFamily"
```

```python
# SavingsPlanRatePropertyKeyType definition
SavingsPlanRatePropertyKeyType = Literal[
    "instanceFamily",
    "instanceType",
    "productDescription",
    "region",
    "tenancy",
]
```
## SavingsPlanRateServiceCodeType

```python
# SavingsPlanRateServiceCodeType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanRateServiceCodeType

def get_value() -> SavingsPlanRateServiceCodeType:
    return "AWSDatabaseMigrationSvc"
```

```python
# SavingsPlanRateServiceCodeType definition
SavingsPlanRateServiceCodeType = Literal[
    "AmazonDocDB",
    "AmazonDynamoDB",
    "AmazonEC2",
    "AmazonECS",
    "AmazonEKS",
    "AmazonElastiCache",
    "AmazonMCS",
    "AmazonNeptune",
    "AmazonRDS",
    "AmazonSageMaker",
    "AmazonTimestream",
    "AuroraDSQL",
    "AWSDatabaseMigrationSvc",
    "AWSLambda",
]
```
## SavingsPlanRateUnitType

```python
# SavingsPlanRateUnitType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanRateUnitType

def get_value() -> SavingsPlanRateUnitType:
    return "ACU-Hr"
```

```python
# SavingsPlanRateUnitType definition
SavingsPlanRateUnitType = Literal[
    "ACU-Hr",
    "DCU-Hr",
    "DPU",
    "ElastiCacheProcessingUnit",
    "GB-Hours",
    "Hrs",
    "Lambda-GB-Second",
    "NCU-hr",
    "ReadCapacityUnit-Hrs",
    "ReadRequestUnits",
    "ReplicatedWriteCapacityUnit-Hrs",
    "ReplicatedWriteRequestUnits",
    "Request",
    "WriteCapacityUnit-Hrs",
    "WriteRequestUnits",
]
```
## SavingsPlanStateType

```python
# SavingsPlanStateType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanStateType

def get_value() -> SavingsPlanStateType:
    return "active"
```

```python
# SavingsPlanStateType definition
SavingsPlanStateType = Literal[
    "active",
    "payment-failed",
    "payment-pending",
    "pending-return",
    "queued",
    "queued-deleted",
    "retired",
    "returned",
]
```
## SavingsPlanTypeType

```python
# SavingsPlanTypeType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlanTypeType

def get_value() -> SavingsPlanTypeType:
    return "Compute"
```

```python
# SavingsPlanTypeType definition
SavingsPlanTypeType = Literal[
    "Compute",
    "Database",
    "EC2Instance",
    "SageMaker",
]
```
## SavingsPlansFilterNameType

```python
# SavingsPlansFilterNameType usage example
from types_aiobotocore_savingsplans.literals import SavingsPlansFilterNameType

def get_value() -> SavingsPlansFilterNameType:
    return "commitment"
```

```python
# SavingsPlansFilterNameType definition
SavingsPlansFilterNameType = Literal[
    "commitment",
    "ec2-instance-family",
    "end",
    "instance-family",
    "payment-option",
    "region",
    "savings-plan-type",
    "start",
    "term",
    "upfront",
]
```
## SavingsPlansServiceName

```python
# SavingsPlansServiceName usage example
from types_aiobotocore_savingsplans.literals import SavingsPlansServiceName

def get_value() -> SavingsPlansServiceName:
    return "savingsplans"
```

```python
# SavingsPlansServiceName definition
SavingsPlansServiceName = Literal[
    "savingsplans",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_savingsplans.literals import ServiceName

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
from types_aiobotocore_savingsplans.literals import ResourceServiceName

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
