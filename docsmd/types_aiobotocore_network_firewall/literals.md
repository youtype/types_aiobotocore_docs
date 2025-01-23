# Literals

> [Index](../README.md) > [NetworkFirewall](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#networkfirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## AttachmentStatusType

```python
# AttachmentStatusType usage example

from types_aiobotocore_network_firewall.literals import AttachmentStatusType

def get_value() -> AttachmentStatusType:
    return "CREATING"
```

```python
# AttachmentStatusType definition

AttachmentStatusType = Literal[
    "CREATING",
    "DELETING",
    "ERROR",
    "FAILED",
    "READY",
    "SCALING",
]
```
## ConfigurationSyncStateType

```python
# ConfigurationSyncStateType usage example

from types_aiobotocore_network_firewall.literals import ConfigurationSyncStateType

def get_value() -> ConfigurationSyncStateType:
    return "CAPACITY_CONSTRAINED"
```

```python
# ConfigurationSyncStateType definition

ConfigurationSyncStateType = Literal[
    "CAPACITY_CONSTRAINED",
    "IN_SYNC",
    "PENDING",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example

from types_aiobotocore_network_firewall.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "AWS_OWNED_KMS_KEY"
```

```python
# EncryptionTypeType definition

EncryptionTypeType = Literal[
    "AWS_OWNED_KMS_KEY",
    "CUSTOMER_KMS",
]
```
## FirewallStatusValueType

```python
# FirewallStatusValueType usage example

from types_aiobotocore_network_firewall.literals import FirewallStatusValueType

def get_value() -> FirewallStatusValueType:
    return "DELETING"
```

```python
# FirewallStatusValueType definition

FirewallStatusValueType = Literal[
    "DELETING",
    "PROVISIONING",
    "READY",
]
```
## GeneratedRulesTypeType

```python
# GeneratedRulesTypeType usage example

from types_aiobotocore_network_firewall.literals import GeneratedRulesTypeType

def get_value() -> GeneratedRulesTypeType:
    return "ALLOWLIST"
```

```python
# GeneratedRulesTypeType definition

GeneratedRulesTypeType = Literal[
    "ALLOWLIST",
    "DENYLIST",
]
```
## IPAddressTypeType

```python
# IPAddressTypeType usage example

from types_aiobotocore_network_firewall.literals import IPAddressTypeType

def get_value() -> IPAddressTypeType:
    return "DUALSTACK"
```

```python
# IPAddressTypeType definition

IPAddressTypeType = Literal[
    "DUALSTACK",
    "IPV4",
    "IPV6",
]
```
## IdentifiedTypeType

```python
# IdentifiedTypeType usage example

from types_aiobotocore_network_firewall.literals import IdentifiedTypeType

def get_value() -> IdentifiedTypeType:
    return "STATELESS_RULE_CONTAINS_TCP_FLAGS"
```

```python
# IdentifiedTypeType definition

IdentifiedTypeType = Literal[
    "STATELESS_RULE_CONTAINS_TCP_FLAGS",
    "STATELESS_RULE_FORWARDING_ASYMMETRICALLY",
]
```
## ListFirewallPoliciesPaginatorName

```python
# ListFirewallPoliciesPaginatorName usage example

from types_aiobotocore_network_firewall.literals import ListFirewallPoliciesPaginatorName

def get_value() -> ListFirewallPoliciesPaginatorName:
    return "list_firewall_policies"
```

```python
# ListFirewallPoliciesPaginatorName definition

ListFirewallPoliciesPaginatorName = Literal[
    "list_firewall_policies",
]
```
## ListFirewallsPaginatorName

```python
# ListFirewallsPaginatorName usage example

from types_aiobotocore_network_firewall.literals import ListFirewallsPaginatorName

def get_value() -> ListFirewallsPaginatorName:
    return "list_firewalls"
```

```python
# ListFirewallsPaginatorName definition

ListFirewallsPaginatorName = Literal[
    "list_firewalls",
]
```
## ListRuleGroupsPaginatorName

```python
# ListRuleGroupsPaginatorName usage example

from types_aiobotocore_network_firewall.literals import ListRuleGroupsPaginatorName

def get_value() -> ListRuleGroupsPaginatorName:
    return "list_rule_groups"
```

```python
# ListRuleGroupsPaginatorName definition

ListRuleGroupsPaginatorName = Literal[
    "list_rule_groups",
]
```
## ListTLSInspectionConfigurationsPaginatorName

```python
# ListTLSInspectionConfigurationsPaginatorName usage example

from types_aiobotocore_network_firewall.literals import ListTLSInspectionConfigurationsPaginatorName

def get_value() -> ListTLSInspectionConfigurationsPaginatorName:
    return "list_tls_inspection_configurations"
```

```python
# ListTLSInspectionConfigurationsPaginatorName definition

ListTLSInspectionConfigurationsPaginatorName = Literal[
    "list_tls_inspection_configurations",
]
```
## ListTagsForResourcePaginatorName

```python
# ListTagsForResourcePaginatorName usage example

from types_aiobotocore_network_firewall.literals import ListTagsForResourcePaginatorName

def get_value() -> ListTagsForResourcePaginatorName:
    return "list_tags_for_resource"
```

```python
# ListTagsForResourcePaginatorName definition

ListTagsForResourcePaginatorName = Literal[
    "list_tags_for_resource",
]
```
## LogDestinationTypeType

```python
# LogDestinationTypeType usage example

from types_aiobotocore_network_firewall.literals import LogDestinationTypeType

def get_value() -> LogDestinationTypeType:
    return "CloudWatchLogs"
```

```python
# LogDestinationTypeType definition

LogDestinationTypeType = Literal[
    "CloudWatchLogs",
    "KinesisDataFirehose",
    "S3",
]
```
## LogTypeType

```python
# LogTypeType usage example

from types_aiobotocore_network_firewall.literals import LogTypeType

def get_value() -> LogTypeType:
    return "ALERT"
```

```python
# LogTypeType definition

LogTypeType = Literal[
    "ALERT",
    "FLOW",
    "TLS",
]
```
## OverrideActionType

```python
# OverrideActionType usage example

from types_aiobotocore_network_firewall.literals import OverrideActionType

def get_value() -> OverrideActionType:
    return "DROP_TO_ALERT"
```

```python
# OverrideActionType definition

OverrideActionType = Literal[
    "DROP_TO_ALERT",
]
```
## PerObjectSyncStatusType

```python
# PerObjectSyncStatusType usage example

from types_aiobotocore_network_firewall.literals import PerObjectSyncStatusType

def get_value() -> PerObjectSyncStatusType:
    return "CAPACITY_CONSTRAINED"
```

```python
# PerObjectSyncStatusType definition

PerObjectSyncStatusType = Literal[
    "CAPACITY_CONSTRAINED",
    "IN_SYNC",
    "PENDING",
]
```
## ResourceManagedStatusType

```python
# ResourceManagedStatusType usage example

from types_aiobotocore_network_firewall.literals import ResourceManagedStatusType

def get_value() -> ResourceManagedStatusType:
    return "ACCOUNT"
```

```python
# ResourceManagedStatusType definition

ResourceManagedStatusType = Literal[
    "ACCOUNT",
    "MANAGED",
]
```
## ResourceManagedTypeType

```python
# ResourceManagedTypeType usage example

from types_aiobotocore_network_firewall.literals import ResourceManagedTypeType

def get_value() -> ResourceManagedTypeType:
    return "AWS_MANAGED_DOMAIN_LISTS"
```

```python
# ResourceManagedTypeType definition

ResourceManagedTypeType = Literal[
    "AWS_MANAGED_DOMAIN_LISTS",
    "AWS_MANAGED_THREAT_SIGNATURES",
]
```
## ResourceStatusType

```python
# ResourceStatusType usage example

from types_aiobotocore_network_firewall.literals import ResourceStatusType

def get_value() -> ResourceStatusType:
    return "ACTIVE"
```

```python
# ResourceStatusType definition

ResourceStatusType = Literal[
    "ACTIVE",
    "DELETING",
    "ERROR",
]
```
## RevocationCheckActionType

```python
# RevocationCheckActionType usage example

from types_aiobotocore_network_firewall.literals import RevocationCheckActionType

def get_value() -> RevocationCheckActionType:
    return "DROP"
```

```python
# RevocationCheckActionType definition

RevocationCheckActionType = Literal[
    "DROP",
    "PASS",
    "REJECT",
]
```
## RuleGroupTypeType

```python
# RuleGroupTypeType usage example

from types_aiobotocore_network_firewall.literals import RuleGroupTypeType

def get_value() -> RuleGroupTypeType:
    return "STATEFUL"
```

```python
# RuleGroupTypeType definition

RuleGroupTypeType = Literal[
    "STATEFUL",
    "STATELESS",
]
```
## RuleOrderType

```python
# RuleOrderType usage example

from types_aiobotocore_network_firewall.literals import RuleOrderType

def get_value() -> RuleOrderType:
    return "DEFAULT_ACTION_ORDER"
```

```python
# RuleOrderType definition

RuleOrderType = Literal[
    "DEFAULT_ACTION_ORDER",
    "STRICT_ORDER",
]
```
## StatefulActionType

```python
# StatefulActionType usage example

from types_aiobotocore_network_firewall.literals import StatefulActionType

def get_value() -> StatefulActionType:
    return "ALERT"
```

```python
# StatefulActionType definition

StatefulActionType = Literal[
    "ALERT",
    "DROP",
    "PASS",
    "REJECT",
]
```
## StatefulRuleDirectionType

```python
# StatefulRuleDirectionType usage example

from types_aiobotocore_network_firewall.literals import StatefulRuleDirectionType

def get_value() -> StatefulRuleDirectionType:
    return "ANY"
```

```python
# StatefulRuleDirectionType definition

StatefulRuleDirectionType = Literal[
    "ANY",
    "FORWARD",
]
```
## StatefulRuleProtocolType

```python
# StatefulRuleProtocolType usage example

from types_aiobotocore_network_firewall.literals import StatefulRuleProtocolType

def get_value() -> StatefulRuleProtocolType:
    return "DCERPC"
```

```python
# StatefulRuleProtocolType definition

StatefulRuleProtocolType = Literal[
    "DCERPC",
    "DHCP",
    "DNS",
    "FTP",
    "HTTP",
    "ICMP",
    "IKEV2",
    "IMAP",
    "IP",
    "KRB5",
    "MSN",
    "NTP",
    "SMB",
    "SMTP",
    "SSH",
    "TCP",
    "TFTP",
    "TLS",
    "UDP",
]
```
## StreamExceptionPolicyType

```python
# StreamExceptionPolicyType usage example

from types_aiobotocore_network_firewall.literals import StreamExceptionPolicyType

def get_value() -> StreamExceptionPolicyType:
    return "CONTINUE"
```

```python
# StreamExceptionPolicyType definition

StreamExceptionPolicyType = Literal[
    "CONTINUE",
    "DROP",
    "REJECT",
]
```
## TCPFlagType

```python
# TCPFlagType usage example

from types_aiobotocore_network_firewall.literals import TCPFlagType

def get_value() -> TCPFlagType:
    return "ACK"
```

```python
# TCPFlagType definition

TCPFlagType = Literal[
    "ACK",
    "CWR",
    "ECE",
    "FIN",
    "PSH",
    "RST",
    "SYN",
    "URG",
]
```
## TargetTypeType

```python
# TargetTypeType usage example

from types_aiobotocore_network_firewall.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "HTTP_HOST"
```

```python
# TargetTypeType definition

TargetTypeType = Literal[
    "HTTP_HOST",
    "TLS_SNI",
]
```
## NetworkFirewallServiceName

```python
# NetworkFirewallServiceName usage example

from types_aiobotocore_network_firewall.literals import NetworkFirewallServiceName

def get_value() -> NetworkFirewallServiceName:
    return "network-firewall"
```

```python
# NetworkFirewallServiceName definition

NetworkFirewallServiceName = Literal[
    "network-firewall",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_network_firewall.literals import ServiceName

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

from types_aiobotocore_network_firewall.literals import ResourceServiceName

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

from types_aiobotocore_network_firewall.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_firewall_policies"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_firewall_policies",
    "list_firewalls",
    "list_rule_groups",
    "list_tags_for_resource",
    "list_tls_inspection_configurations",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_network_firewall.literals import RegionName

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
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ap-southeast-5",
    "ca-central-1",
    "ca-west-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
