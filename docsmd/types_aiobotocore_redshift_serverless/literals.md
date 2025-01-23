# Literals

> [Index](../README.md) > [RedshiftServerless](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#redshiftserverless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## ListCustomDomainAssociationsPaginatorName

```python
# ListCustomDomainAssociationsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListCustomDomainAssociationsPaginatorName

def get_value() -> ListCustomDomainAssociationsPaginatorName:
    return "list_custom_domain_associations"
```

```python
# ListCustomDomainAssociationsPaginatorName definition

ListCustomDomainAssociationsPaginatorName = Literal[
    "list_custom_domain_associations",
]
```
## ListEndpointAccessPaginatorName

```python
# ListEndpointAccessPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListEndpointAccessPaginatorName

def get_value() -> ListEndpointAccessPaginatorName:
    return "list_endpoint_access"
```

```python
# ListEndpointAccessPaginatorName definition

ListEndpointAccessPaginatorName = Literal[
    "list_endpoint_access",
]
```
## ListManagedWorkgroupsPaginatorName

```python
# ListManagedWorkgroupsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListManagedWorkgroupsPaginatorName

def get_value() -> ListManagedWorkgroupsPaginatorName:
    return "list_managed_workgroups"
```

```python
# ListManagedWorkgroupsPaginatorName definition

ListManagedWorkgroupsPaginatorName = Literal[
    "list_managed_workgroups",
]
```
## ListNamespacesPaginatorName

```python
# ListNamespacesPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListNamespacesPaginatorName

def get_value() -> ListNamespacesPaginatorName:
    return "list_namespaces"
```

```python
# ListNamespacesPaginatorName definition

ListNamespacesPaginatorName = Literal[
    "list_namespaces",
]
```
## ListRecoveryPointsPaginatorName

```python
# ListRecoveryPointsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListRecoveryPointsPaginatorName

def get_value() -> ListRecoveryPointsPaginatorName:
    return "list_recovery_points"
```

```python
# ListRecoveryPointsPaginatorName definition

ListRecoveryPointsPaginatorName = Literal[
    "list_recovery_points",
]
```
## ListScheduledActionsPaginatorName

```python
# ListScheduledActionsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListScheduledActionsPaginatorName

def get_value() -> ListScheduledActionsPaginatorName:
    return "list_scheduled_actions"
```

```python
# ListScheduledActionsPaginatorName definition

ListScheduledActionsPaginatorName = Literal[
    "list_scheduled_actions",
]
```
## ListSnapshotCopyConfigurationsPaginatorName

```python
# ListSnapshotCopyConfigurationsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListSnapshotCopyConfigurationsPaginatorName

def get_value() -> ListSnapshotCopyConfigurationsPaginatorName:
    return "list_snapshot_copy_configurations"
```

```python
# ListSnapshotCopyConfigurationsPaginatorName definition

ListSnapshotCopyConfigurationsPaginatorName = Literal[
    "list_snapshot_copy_configurations",
]
```
## ListSnapshotsPaginatorName

```python
# ListSnapshotsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListSnapshotsPaginatorName

def get_value() -> ListSnapshotsPaginatorName:
    return "list_snapshots"
```

```python
# ListSnapshotsPaginatorName definition

ListSnapshotsPaginatorName = Literal[
    "list_snapshots",
]
```
## ListTableRestoreStatusPaginatorName

```python
# ListTableRestoreStatusPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListTableRestoreStatusPaginatorName

def get_value() -> ListTableRestoreStatusPaginatorName:
    return "list_table_restore_status"
```

```python
# ListTableRestoreStatusPaginatorName definition

ListTableRestoreStatusPaginatorName = Literal[
    "list_table_restore_status",
]
```
## ListUsageLimitsPaginatorName

```python
# ListUsageLimitsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListUsageLimitsPaginatorName

def get_value() -> ListUsageLimitsPaginatorName:
    return "list_usage_limits"
```

```python
# ListUsageLimitsPaginatorName definition

ListUsageLimitsPaginatorName = Literal[
    "list_usage_limits",
]
```
## ListWorkgroupsPaginatorName

```python
# ListWorkgroupsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListWorkgroupsPaginatorName

def get_value() -> ListWorkgroupsPaginatorName:
    return "list_workgroups"
```

```python
# ListWorkgroupsPaginatorName definition

ListWorkgroupsPaginatorName = Literal[
    "list_workgroups",
]
```
## LogExportType

```python
# LogExportType usage example

from types_aiobotocore_redshift_serverless.literals import LogExportType

def get_value() -> LogExportType:
    return "connectionlog"
```

```python
# LogExportType definition

LogExportType = Literal[
    "connectionlog",
    "useractivitylog",
    "userlog",
]
```
## ManagedWorkgroupStatusType

```python
# ManagedWorkgroupStatusType usage example

from types_aiobotocore_redshift_serverless.literals import ManagedWorkgroupStatusType

def get_value() -> ManagedWorkgroupStatusType:
    return "AVAILABLE"
```

```python
# ManagedWorkgroupStatusType definition

ManagedWorkgroupStatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "MODIFYING",
    "NOT_AVAILABLE",
]
```
## NamespaceStatusType

```python
# NamespaceStatusType usage example

from types_aiobotocore_redshift_serverless.literals import NamespaceStatusType

def get_value() -> NamespaceStatusType:
    return "AVAILABLE"
```

```python
# NamespaceStatusType definition

NamespaceStatusType = Literal[
    "AVAILABLE",
    "DELETING",
    "MODIFYING",
]
```
## PerformanceTargetStatusType

```python
# PerformanceTargetStatusType usage example

from types_aiobotocore_redshift_serverless.literals import PerformanceTargetStatusType

def get_value() -> PerformanceTargetStatusType:
    return "DISABLED"
```

```python
# PerformanceTargetStatusType definition

PerformanceTargetStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## SnapshotStatusType

```python
# SnapshotStatusType usage example

from types_aiobotocore_redshift_serverless.literals import SnapshotStatusType

def get_value() -> SnapshotStatusType:
    return "AVAILABLE"
```

```python
# SnapshotStatusType definition

SnapshotStatusType = Literal[
    "AVAILABLE",
    "CANCELLED",
    "COPYING",
    "CREATING",
    "DELETED",
    "FAILED",
]
```
## StateType

```python
# StateType usage example

from types_aiobotocore_redshift_serverless.literals import StateType

def get_value() -> StateType:
    return "ACTIVE"
```

```python
# StateType definition

StateType = Literal[
    "ACTIVE",
    "DISABLED",
]
```
## UsageLimitBreachActionType

```python
# UsageLimitBreachActionType usage example

from types_aiobotocore_redshift_serverless.literals import UsageLimitBreachActionType

def get_value() -> UsageLimitBreachActionType:
    return "deactivate"
```

```python
# UsageLimitBreachActionType definition

UsageLimitBreachActionType = Literal[
    "deactivate",
    "emit-metric",
    "log",
]
```
## UsageLimitPeriodType

```python
# UsageLimitPeriodType usage example

from types_aiobotocore_redshift_serverless.literals import UsageLimitPeriodType

def get_value() -> UsageLimitPeriodType:
    return "daily"
```

```python
# UsageLimitPeriodType definition

UsageLimitPeriodType = Literal[
    "daily",
    "monthly",
    "weekly",
]
```
## UsageLimitUsageTypeType

```python
# UsageLimitUsageTypeType usage example

from types_aiobotocore_redshift_serverless.literals import UsageLimitUsageTypeType

def get_value() -> UsageLimitUsageTypeType:
    return "cross-region-datasharing"
```

```python
# UsageLimitUsageTypeType definition

UsageLimitUsageTypeType = Literal[
    "cross-region-datasharing",
    "serverless-compute",
]
```
## WorkgroupStatusType

```python
# WorkgroupStatusType usage example

from types_aiobotocore_redshift_serverless.literals import WorkgroupStatusType

def get_value() -> WorkgroupStatusType:
    return "AVAILABLE"
```

```python
# WorkgroupStatusType definition

WorkgroupStatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "MODIFYING",
]
```
## RedshiftServerlessServiceName

```python
# RedshiftServerlessServiceName usage example

from types_aiobotocore_redshift_serverless.literals import RedshiftServerlessServiceName

def get_value() -> RedshiftServerlessServiceName:
    return "redshift-serverless"
```

```python
# RedshiftServerlessServiceName definition

RedshiftServerlessServiceName = Literal[
    "redshift-serverless",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_redshift_serverless.literals import ServiceName

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

from types_aiobotocore_redshift_serverless.literals import ResourceServiceName

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

from types_aiobotocore_redshift_serverless.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_custom_domain_associations"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_custom_domain_associations",
    "list_endpoint_access",
    "list_managed_workgroups",
    "list_namespaces",
    "list_recovery_points",
    "list_scheduled_actions",
    "list_snapshot_copy_configurations",
    "list_snapshots",
    "list_table_restore_status",
    "list_usage_limits",
    "list_workgroups",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_redshift_serverless.literals import RegionName

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
    "ap-southeast-3",
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
