# Literals

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## DukptDerivationTypeType

```python
# DukptDerivationTypeType usage example

from types_aiobotocore_payment_cryptography_data.literals import DukptDerivationTypeType

def get_value() -> DukptDerivationTypeType:
    return "AES_128"
```

```python
# DukptDerivationTypeType definition

DukptDerivationTypeType = Literal[
    "AES_128",
    "AES_192",
    "AES_256",
    "TDES_2KEY",
    "TDES_3KEY",
]
```
## DukptEncryptionModeType

```python
# DukptEncryptionModeType usage example

from types_aiobotocore_payment_cryptography_data.literals import DukptEncryptionModeType

def get_value() -> DukptEncryptionModeType:
    return "CBC"
```

```python
# DukptEncryptionModeType definition

DukptEncryptionModeType = Literal[
    "CBC",
    "ECB",
]
```
## DukptKeyVariantType

```python
# DukptKeyVariantType usage example

from types_aiobotocore_payment_cryptography_data.literals import DukptKeyVariantType

def get_value() -> DukptKeyVariantType:
    return "BIDIRECTIONAL"
```

```python
# DukptKeyVariantType definition

DukptKeyVariantType = Literal[
    "BIDIRECTIONAL",
    "REQUEST",
    "RESPONSE",
]
```
## EncryptionModeType

```python
# EncryptionModeType usage example

from types_aiobotocore_payment_cryptography_data.literals import EncryptionModeType

def get_value() -> EncryptionModeType:
    return "CBC"
```

```python
# EncryptionModeType definition

EncryptionModeType = Literal[
    "CBC",
    "CFB",
    "CFB1",
    "CFB128",
    "CFB64",
    "CFB8",
    "ECB",
    "OFB",
]
```
## MacAlgorithmType

```python
# MacAlgorithmType usage example

from types_aiobotocore_payment_cryptography_data.literals import MacAlgorithmType

def get_value() -> MacAlgorithmType:
    return "CMAC"
```

```python
# MacAlgorithmType definition

MacAlgorithmType = Literal[
    "CMAC",
    "HMAC_SHA224",
    "HMAC_SHA256",
    "HMAC_SHA384",
    "HMAC_SHA512",
    "ISO9797_ALGORITHM1",
    "ISO9797_ALGORITHM3",
]
```
## MajorKeyDerivationModeType

```python
# MajorKeyDerivationModeType usage example

from types_aiobotocore_payment_cryptography_data.literals import MajorKeyDerivationModeType

def get_value() -> MajorKeyDerivationModeType:
    return "EMV_OPTION_A"
```

```python
# MajorKeyDerivationModeType definition

MajorKeyDerivationModeType = Literal[
    "EMV_OPTION_A",
    "EMV_OPTION_B",
]
```
## PaddingTypeType

```python
# PaddingTypeType usage example

from types_aiobotocore_payment_cryptography_data.literals import PaddingTypeType

def get_value() -> PaddingTypeType:
    return "OAEP_SHA1"
```

```python
# PaddingTypeType definition

PaddingTypeType = Literal[
    "OAEP_SHA1",
    "OAEP_SHA256",
    "OAEP_SHA512",
    "PKCS1",
]
```
## PinBlockFormatForPinDataType

```python
# PinBlockFormatForPinDataType usage example

from types_aiobotocore_payment_cryptography_data.literals import PinBlockFormatForPinDataType

def get_value() -> PinBlockFormatForPinDataType:
    return "ISO_FORMAT_0"
```

```python
# PinBlockFormatForPinDataType definition

PinBlockFormatForPinDataType = Literal[
    "ISO_FORMAT_0",
    "ISO_FORMAT_3",
]
```
## SessionKeyDerivationModeType

```python
# SessionKeyDerivationModeType usage example

from types_aiobotocore_payment_cryptography_data.literals import SessionKeyDerivationModeType

def get_value() -> SessionKeyDerivationModeType:
    return "AMEX"
```

```python
# SessionKeyDerivationModeType definition

SessionKeyDerivationModeType = Literal[
    "AMEX",
    "EMV2000",
    "EMV_COMMON_SESSION_KEY",
    "MASTERCARD_SESSION_KEY",
    "VISA",
]
```
## PaymentCryptographyDataPlaneServiceName

```python
# PaymentCryptographyDataPlaneServiceName usage example

from types_aiobotocore_payment_cryptography_data.literals import PaymentCryptographyDataPlaneServiceName

def get_value() -> PaymentCryptographyDataPlaneServiceName:
    return "payment-cryptography-data"
```

```python
# PaymentCryptographyDataPlaneServiceName definition

PaymentCryptographyDataPlaneServiceName = Literal[
    "payment-cryptography-data",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_payment_cryptography_data.literals import ServiceName

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

from types_aiobotocore_payment_cryptography_data.literals import ResourceServiceName

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
