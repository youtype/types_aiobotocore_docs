# Literals

> [Index](../README.md) > [TaxSettings](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## AddressRoleTypeType

```python
# AddressRoleTypeType usage example

from types_aiobotocore_taxsettings.literals import AddressRoleTypeType

def get_value() -> AddressRoleTypeType:
    return "BillingAddress"
```

```python
# AddressRoleTypeType definition

AddressRoleTypeType = Literal[
    "BillingAddress",
    "ContactAddress",
    "TaxAddress",
]
```
## IndustriesType

```python
# IndustriesType usage example

from types_aiobotocore_taxsettings.literals import IndustriesType

def get_value() -> IndustriesType:
    return "Banks"
```

```python
# IndustriesType definition

IndustriesType = Literal[
    "Banks",
    "CirculatingOrg",
    "DevelopmentAgencies",
    "Insurance",
    "PensionAndBenefitFunds",
    "ProfessionalOrg",
]
```
## IsraelCustomerTypeType

```python
# IsraelCustomerTypeType usage example

from types_aiobotocore_taxsettings.literals import IsraelCustomerTypeType

def get_value() -> IsraelCustomerTypeType:
    return "Business"
```

```python
# IsraelCustomerTypeType definition

IsraelCustomerTypeType = Literal[
    "Business",
    "Individual",
]
```
## IsraelDealerTypeType

```python
# IsraelDealerTypeType usage example

from types_aiobotocore_taxsettings.literals import IsraelDealerTypeType

def get_value() -> IsraelDealerTypeType:
    return "Authorized"
```

```python
# IsraelDealerTypeType definition

IsraelDealerTypeType = Literal[
    "Authorized",
    "Non-authorized",
]
```
## ListTaxRegistrationsPaginatorName

```python
# ListTaxRegistrationsPaginatorName usage example

from types_aiobotocore_taxsettings.literals import ListTaxRegistrationsPaginatorName

def get_value() -> ListTaxRegistrationsPaginatorName:
    return "list_tax_registrations"
```

```python
# ListTaxRegistrationsPaginatorName definition

ListTaxRegistrationsPaginatorName = Literal[
    "list_tax_registrations",
]
```
## MalaysiaServiceTaxCodeType

```python
# MalaysiaServiceTaxCodeType usage example

from types_aiobotocore_taxsettings.literals import MalaysiaServiceTaxCodeType

def get_value() -> MalaysiaServiceTaxCodeType:
    return "Consultancy"
```

```python
# MalaysiaServiceTaxCodeType definition

MalaysiaServiceTaxCodeType = Literal[
    "Consultancy",
    "Digital Service And Electronic Medium",
    "IT Services",
    "Training Or Coaching",
]
```
## PersonTypeType

```python
# PersonTypeType usage example

from types_aiobotocore_taxsettings.literals import PersonTypeType

def get_value() -> PersonTypeType:
    return "Business"
```

```python
# PersonTypeType definition

PersonTypeType = Literal[
    "Business",
    "Legal Person",
    "Physical Person",
]
```
## RegistrationTypeType

```python
# RegistrationTypeType usage example

from types_aiobotocore_taxsettings.literals import RegistrationTypeType

def get_value() -> RegistrationTypeType:
    return "Intra-EU"
```

```python
# RegistrationTypeType definition

RegistrationTypeType = Literal[
    "Intra-EU",
    "Local",
]
```
## SaudiArabiaTaxRegistrationNumberTypeType

```python
# SaudiArabiaTaxRegistrationNumberTypeType usage example

from types_aiobotocore_taxsettings.literals import SaudiArabiaTaxRegistrationNumberTypeType

def get_value() -> SaudiArabiaTaxRegistrationNumberTypeType:
    return "CommercialRegistrationNumber"
```

```python
# SaudiArabiaTaxRegistrationNumberTypeType definition

SaudiArabiaTaxRegistrationNumberTypeType = Literal[
    "CommercialRegistrationNumber",
    "TaxIdentificationNumber",
    "TaxRegistrationNumber",
]
```
## SectorType

```python
# SectorType usage example

from types_aiobotocore_taxsettings.literals import SectorType

def get_value() -> SectorType:
    return "Business"
```

```python
# SectorType definition

SectorType = Literal[
    "Business",
    "Government",
    "Individual",
]
```
## TaxRegistrationNumberTypeType

```python
# TaxRegistrationNumberTypeType usage example

from types_aiobotocore_taxsettings.literals import TaxRegistrationNumberTypeType

def get_value() -> TaxRegistrationNumberTypeType:
    return "LocalRegistrationNumber"
```

```python
# TaxRegistrationNumberTypeType definition

TaxRegistrationNumberTypeType = Literal[
    "LocalRegistrationNumber",
    "TaxRegistrationNumber",
]
```
## TaxRegistrationStatusType

```python
# TaxRegistrationStatusType usage example

from types_aiobotocore_taxsettings.literals import TaxRegistrationStatusType

def get_value() -> TaxRegistrationStatusType:
    return "Deleted"
```

```python
# TaxRegistrationStatusType definition

TaxRegistrationStatusType = Literal[
    "Deleted",
    "Pending",
    "Rejected",
    "Verified",
]
```
## TaxRegistrationTypeType

```python
# TaxRegistrationTypeType usage example

from types_aiobotocore_taxsettings.literals import TaxRegistrationTypeType

def get_value() -> TaxRegistrationTypeType:
    return "CNPJ"
```

```python
# TaxRegistrationTypeType definition

TaxRegistrationTypeType = Literal[
    "CNPJ",
    "CPF",
    "GST",
    "SST",
    "VAT",
]
```
## UkraineTrnTypeType

```python
# UkraineTrnTypeType usage example

from types_aiobotocore_taxsettings.literals import UkraineTrnTypeType

def get_value() -> UkraineTrnTypeType:
    return "Business"
```

```python
# UkraineTrnTypeType definition

UkraineTrnTypeType = Literal[
    "Business",
    "Individual",
]
```
## TaxSettingsServiceName

```python
# TaxSettingsServiceName usage example

from types_aiobotocore_taxsettings.literals import TaxSettingsServiceName

def get_value() -> TaxSettingsServiceName:
    return "taxsettings"
```

```python
# TaxSettingsServiceName definition

TaxSettingsServiceName = Literal[
    "taxsettings",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_taxsettings.literals import ServiceName

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
    "batch",
    "bcm-data-exports",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-runtime",
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
    "iot",
    "iot-data",
    "iot-jobs-data",
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
    "networkmanager",
    "networkmonitor",
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

from types_aiobotocore_taxsettings.literals import ResourceServiceName

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

from types_aiobotocore_taxsettings.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_tax_registrations"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_tax_registrations",
]
```
