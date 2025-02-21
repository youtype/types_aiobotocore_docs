# Literals

> [Index](../README.md) > [MainframeModernizationApplicationTesting](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## CaptureToolType

```python
# CaptureToolType usage example
from types_aiobotocore_apptest.literals import CaptureToolType

def get_value() -> CaptureToolType:
    return "AWS DMS"
```

```python
# CaptureToolType definition
CaptureToolType = Literal[
    "AWS DMS",
    "Precisely",
]
```
## CloudFormationActionTypeType

```python
# CloudFormationActionTypeType usage example
from types_aiobotocore_apptest.literals import CloudFormationActionTypeType

def get_value() -> CloudFormationActionTypeType:
    return "Create"
```

```python
# CloudFormationActionTypeType definition
CloudFormationActionTypeType = Literal[
    "Create",
    "Delete",
]
```
## ComparisonStatusEnumType

```python
# ComparisonStatusEnumType usage example
from types_aiobotocore_apptest.literals import ComparisonStatusEnumType

def get_value() -> ComparisonStatusEnumType:
    return "Different"
```

```python
# ComparisonStatusEnumType definition
ComparisonStatusEnumType = Literal[
    "Different",
    "Equal",
    "Equivalent",
]
```
## DataSetTypeType

```python
# DataSetTypeType usage example
from types_aiobotocore_apptest.literals import DataSetTypeType

def get_value() -> DataSetTypeType:
    return "PS"
```

```python
# DataSetTypeType definition
DataSetTypeType = Literal[
    "PS",
]
```
## FormatType

```python
# FormatType usage example
from types_aiobotocore_apptest.literals import FormatType

def get_value() -> FormatType:
    return "FIXED"
```

```python
# FormatType definition
FormatType = Literal[
    "FIXED",
    "LINE_SEQUENTIAL",
    "VARIABLE",
]
```
## ListTestCasesPaginatorName

```python
# ListTestCasesPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestCasesPaginatorName

def get_value() -> ListTestCasesPaginatorName:
    return "list_test_cases"
```

```python
# ListTestCasesPaginatorName definition
ListTestCasesPaginatorName = Literal[
    "list_test_cases",
]
```
## ListTestConfigurationsPaginatorName

```python
# ListTestConfigurationsPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestConfigurationsPaginatorName

def get_value() -> ListTestConfigurationsPaginatorName:
    return "list_test_configurations"
```

```python
# ListTestConfigurationsPaginatorName definition
ListTestConfigurationsPaginatorName = Literal[
    "list_test_configurations",
]
```
## ListTestRunStepsPaginatorName

```python
# ListTestRunStepsPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestRunStepsPaginatorName

def get_value() -> ListTestRunStepsPaginatorName:
    return "list_test_run_steps"
```

```python
# ListTestRunStepsPaginatorName definition
ListTestRunStepsPaginatorName = Literal[
    "list_test_run_steps",
]
```
## ListTestRunTestCasesPaginatorName

```python
# ListTestRunTestCasesPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestRunTestCasesPaginatorName

def get_value() -> ListTestRunTestCasesPaginatorName:
    return "list_test_run_test_cases"
```

```python
# ListTestRunTestCasesPaginatorName definition
ListTestRunTestCasesPaginatorName = Literal[
    "list_test_run_test_cases",
]
```
## ListTestRunsPaginatorName

```python
# ListTestRunsPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestRunsPaginatorName

def get_value() -> ListTestRunsPaginatorName:
    return "list_test_runs"
```

```python
# ListTestRunsPaginatorName definition
ListTestRunsPaginatorName = Literal[
    "list_test_runs",
]
```
## ListTestSuitesPaginatorName

```python
# ListTestSuitesPaginatorName usage example
from types_aiobotocore_apptest.literals import ListTestSuitesPaginatorName

def get_value() -> ListTestSuitesPaginatorName:
    return "list_test_suites"
```

```python
# ListTestSuitesPaginatorName definition
ListTestSuitesPaginatorName = Literal[
    "list_test_suites",
]
```
## M2ManagedActionTypeType

```python
# M2ManagedActionTypeType usage example
from types_aiobotocore_apptest.literals import M2ManagedActionTypeType

def get_value() -> M2ManagedActionTypeType:
    return "Configure"
```

```python
# M2ManagedActionTypeType definition
M2ManagedActionTypeType = Literal[
    "Configure",
    "Deconfigure",
]
```
## M2ManagedRuntimeType

```python
# M2ManagedRuntimeType usage example
from types_aiobotocore_apptest.literals import M2ManagedRuntimeType

def get_value() -> M2ManagedRuntimeType:
    return "MicroFocus"
```

```python
# M2ManagedRuntimeType definition
M2ManagedRuntimeType = Literal[
    "MicroFocus",
]
```
## M2NonManagedActionTypeType

```python
# M2NonManagedActionTypeType usage example
from types_aiobotocore_apptest.literals import M2NonManagedActionTypeType

def get_value() -> M2NonManagedActionTypeType:
    return "Configure"
```

```python
# M2NonManagedActionTypeType definition
M2NonManagedActionTypeType = Literal[
    "Configure",
    "Deconfigure",
]
```
## M2NonManagedRuntimeType

```python
# M2NonManagedRuntimeType usage example
from types_aiobotocore_apptest.literals import M2NonManagedRuntimeType

def get_value() -> M2NonManagedRuntimeType:
    return "BluAge"
```

```python
# M2NonManagedRuntimeType definition
M2NonManagedRuntimeType = Literal[
    "BluAge",
]
```
## ScriptTypeType

```python
# ScriptTypeType usage example
from types_aiobotocore_apptest.literals import ScriptTypeType

def get_value() -> ScriptTypeType:
    return "Selenium"
```

```python
# ScriptTypeType definition
ScriptTypeType = Literal[
    "Selenium",
]
```
## SourceDatabaseType

```python
# SourceDatabaseType usage example
from types_aiobotocore_apptest.literals import SourceDatabaseType

def get_value() -> SourceDatabaseType:
    return "z/OS-DB2"
```

```python
# SourceDatabaseType definition
SourceDatabaseType = Literal[
    "z/OS-DB2",
]
```
## StepRunStatusType

```python
# StepRunStatusType usage example
from types_aiobotocore_apptest.literals import StepRunStatusType

def get_value() -> StepRunStatusType:
    return "Failed"
```

```python
# StepRunStatusType definition
StepRunStatusType = Literal[
    "Failed",
    "Running",
    "Success",
]
```
## TargetDatabaseType

```python
# TargetDatabaseType usage example
from types_aiobotocore_apptest.literals import TargetDatabaseType

def get_value() -> TargetDatabaseType:
    return "PostgreSQL"
```

```python
# TargetDatabaseType definition
TargetDatabaseType = Literal[
    "PostgreSQL",
]
```
## TestCaseLifecycleType

```python
# TestCaseLifecycleType usage example
from types_aiobotocore_apptest.literals import TestCaseLifecycleType

def get_value() -> TestCaseLifecycleType:
    return "Active"
```

```python
# TestCaseLifecycleType definition
TestCaseLifecycleType = Literal[
    "Active",
    "Deleting",
]
```
## TestCaseRunStatusType

```python
# TestCaseRunStatusType usage example
from types_aiobotocore_apptest.literals import TestCaseRunStatusType

def get_value() -> TestCaseRunStatusType:
    return "Failed"
```

```python
# TestCaseRunStatusType definition
TestCaseRunStatusType = Literal[
    "Failed",
    "Running",
    "Success",
]
```
## TestConfigurationLifecycleType

```python
# TestConfigurationLifecycleType usage example
from types_aiobotocore_apptest.literals import TestConfigurationLifecycleType

def get_value() -> TestConfigurationLifecycleType:
    return "Active"
```

```python
# TestConfigurationLifecycleType definition
TestConfigurationLifecycleType = Literal[
    "Active",
    "Deleting",
]
```
## TestRunStatusType

```python
# TestRunStatusType usage example
from types_aiobotocore_apptest.literals import TestRunStatusType

def get_value() -> TestRunStatusType:
    return "Deleting"
```

```python
# TestRunStatusType definition
TestRunStatusType = Literal[
    "Deleting",
    "Failed",
    "Running",
    "Success",
]
```
## TestSuiteLifecycleType

```python
# TestSuiteLifecycleType usage example
from types_aiobotocore_apptest.literals import TestSuiteLifecycleType

def get_value() -> TestSuiteLifecycleType:
    return "Active"
```

```python
# TestSuiteLifecycleType definition
TestSuiteLifecycleType = Literal[
    "Active",
    "Creating",
    "Deleting",
    "Failed",
    "Updating",
]
```
## MainframeModernizationApplicationTestingServiceName

```python
# MainframeModernizationApplicationTestingServiceName usage example
from types_aiobotocore_apptest.literals import MainframeModernizationApplicationTestingServiceName

def get_value() -> MainframeModernizationApplicationTestingServiceName:
    return "apptest"
```

```python
# MainframeModernizationApplicationTestingServiceName definition
MainframeModernizationApplicationTestingServiceName = Literal[
    "apptest",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_apptest.literals import ServiceName

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
from types_aiobotocore_apptest.literals import ResourceServiceName

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
from types_aiobotocore_apptest.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_test_cases"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_test_cases",
    "list_test_configurations",
    "list_test_run_steps",
    "list_test_run_test_cases",
    "list_test_runs",
    "list_test_suites",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_apptest.literals import RegionName

def get_value() -> RegionName:
    return "ap-southeast-2"
```

```python
# RegionName definition
RegionName = Literal[
    "ap-southeast-2",
    "eu-central-1",
    "sa-east-1",
    "us-east-1",
]
```
