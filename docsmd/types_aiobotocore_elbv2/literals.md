# Literals

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## ActionTypeEnumType

```python
# ActionTypeEnumType usage example

from types_aiobotocore_elbv2.literals import ActionTypeEnumType

def get_value() -> ActionTypeEnumType:
    return "authenticate-cognito"
```

```python
# ActionTypeEnumType definition

ActionTypeEnumType = Literal[
    "authenticate-cognito",
    "authenticate-oidc",
    "fixed-response",
    "forward",
    "redirect",
]
```
## AuthenticateCognitoActionConditionalBehaviorEnumType

```python
# AuthenticateCognitoActionConditionalBehaviorEnumType usage example

from types_aiobotocore_elbv2.literals import AuthenticateCognitoActionConditionalBehaviorEnumType

def get_value() -> AuthenticateCognitoActionConditionalBehaviorEnumType:
    return "allow"
```

```python
# AuthenticateCognitoActionConditionalBehaviorEnumType definition

AuthenticateCognitoActionConditionalBehaviorEnumType = Literal[
    "allow",
    "authenticate",
    "deny",
]
```
## AuthenticateOidcActionConditionalBehaviorEnumType

```python
# AuthenticateOidcActionConditionalBehaviorEnumType usage example

from types_aiobotocore_elbv2.literals import AuthenticateOidcActionConditionalBehaviorEnumType

def get_value() -> AuthenticateOidcActionConditionalBehaviorEnumType:
    return "allow"
```

```python
# AuthenticateOidcActionConditionalBehaviorEnumType definition

AuthenticateOidcActionConditionalBehaviorEnumType = Literal[
    "allow",
    "authenticate",
    "deny",
]
```
## DescribeAccountLimitsPaginatorName

```python
# DescribeAccountLimitsPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeAccountLimitsPaginatorName

def get_value() -> DescribeAccountLimitsPaginatorName:
    return "describe_account_limits"
```

```python
# DescribeAccountLimitsPaginatorName definition

DescribeAccountLimitsPaginatorName = Literal[
    "describe_account_limits",
]
```
## DescribeListenerCertificatesPaginatorName

```python
# DescribeListenerCertificatesPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeListenerCertificatesPaginatorName

def get_value() -> DescribeListenerCertificatesPaginatorName:
    return "describe_listener_certificates"
```

```python
# DescribeListenerCertificatesPaginatorName definition

DescribeListenerCertificatesPaginatorName = Literal[
    "describe_listener_certificates",
]
```
## DescribeListenersPaginatorName

```python
# DescribeListenersPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeListenersPaginatorName

def get_value() -> DescribeListenersPaginatorName:
    return "describe_listeners"
```

```python
# DescribeListenersPaginatorName definition

DescribeListenersPaginatorName = Literal[
    "describe_listeners",
]
```
## DescribeLoadBalancersPaginatorName

```python
# DescribeLoadBalancersPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeLoadBalancersPaginatorName

def get_value() -> DescribeLoadBalancersPaginatorName:
    return "describe_load_balancers"
```

```python
# DescribeLoadBalancersPaginatorName definition

DescribeLoadBalancersPaginatorName = Literal[
    "describe_load_balancers",
]
```
## DescribeRulesPaginatorName

```python
# DescribeRulesPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeRulesPaginatorName

def get_value() -> DescribeRulesPaginatorName:
    return "describe_rules"
```

```python
# DescribeRulesPaginatorName definition

DescribeRulesPaginatorName = Literal[
    "describe_rules",
]
```
## DescribeSSLPoliciesPaginatorName

```python
# DescribeSSLPoliciesPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeSSLPoliciesPaginatorName

def get_value() -> DescribeSSLPoliciesPaginatorName:
    return "describe_ssl_policies"
```

```python
# DescribeSSLPoliciesPaginatorName definition

DescribeSSLPoliciesPaginatorName = Literal[
    "describe_ssl_policies",
]
```
## DescribeTargetGroupsPaginatorName

```python
# DescribeTargetGroupsPaginatorName usage example

from types_aiobotocore_elbv2.literals import DescribeTargetGroupsPaginatorName

def get_value() -> DescribeTargetGroupsPaginatorName:
    return "describe_target_groups"
```

```python
# DescribeTargetGroupsPaginatorName definition

DescribeTargetGroupsPaginatorName = Literal[
    "describe_target_groups",
]
```
## EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType

```python
# EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType usage example

from types_aiobotocore_elbv2.literals import EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType

def get_value() -> EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType:
    return "off"
```

```python
# EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType definition

EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = Literal[
    "off",
    "on",
]
```
## IpAddressTypeType

```python
# IpAddressTypeType usage example

from types_aiobotocore_elbv2.literals import IpAddressTypeType

def get_value() -> IpAddressTypeType:
    return "dualstack"
```

```python
# IpAddressTypeType definition

IpAddressTypeType = Literal[
    "dualstack",
    "ipv4",
]
```
## LoadBalancerAvailableWaiterName

```python
# LoadBalancerAvailableWaiterName usage example

from types_aiobotocore_elbv2.literals import LoadBalancerAvailableWaiterName

def get_value() -> LoadBalancerAvailableWaiterName:
    return "load_balancer_available"
```

```python
# LoadBalancerAvailableWaiterName definition

LoadBalancerAvailableWaiterName = Literal[
    "load_balancer_available",
]
```
## LoadBalancerExistsWaiterName

```python
# LoadBalancerExistsWaiterName usage example

from types_aiobotocore_elbv2.literals import LoadBalancerExistsWaiterName

def get_value() -> LoadBalancerExistsWaiterName:
    return "load_balancer_exists"
```

```python
# LoadBalancerExistsWaiterName definition

LoadBalancerExistsWaiterName = Literal[
    "load_balancer_exists",
]
```
## LoadBalancerSchemeEnumType

```python
# LoadBalancerSchemeEnumType usage example

from types_aiobotocore_elbv2.literals import LoadBalancerSchemeEnumType

def get_value() -> LoadBalancerSchemeEnumType:
    return "internal"
```

```python
# LoadBalancerSchemeEnumType definition

LoadBalancerSchemeEnumType = Literal[
    "internal",
    "internet-facing",
]
```
## LoadBalancerStateEnumType

```python
# LoadBalancerStateEnumType usage example

from types_aiobotocore_elbv2.literals import LoadBalancerStateEnumType

def get_value() -> LoadBalancerStateEnumType:
    return "active"
```

```python
# LoadBalancerStateEnumType definition

LoadBalancerStateEnumType = Literal[
    "active",
    "active_impaired",
    "failed",
    "provisioning",
]
```
## LoadBalancerTypeEnumType

```python
# LoadBalancerTypeEnumType usage example

from types_aiobotocore_elbv2.literals import LoadBalancerTypeEnumType

def get_value() -> LoadBalancerTypeEnumType:
    return "application"
```

```python
# LoadBalancerTypeEnumType definition

LoadBalancerTypeEnumType = Literal[
    "application",
    "gateway",
    "network",
]
```
## LoadBalancersDeletedWaiterName

```python
# LoadBalancersDeletedWaiterName usage example

from types_aiobotocore_elbv2.literals import LoadBalancersDeletedWaiterName

def get_value() -> LoadBalancersDeletedWaiterName:
    return "load_balancers_deleted"
```

```python
# LoadBalancersDeletedWaiterName definition

LoadBalancersDeletedWaiterName = Literal[
    "load_balancers_deleted",
]
```
## ProtocolEnumType

```python
# ProtocolEnumType usage example

from types_aiobotocore_elbv2.literals import ProtocolEnumType

def get_value() -> ProtocolEnumType:
    return "GENEVE"
```

```python
# ProtocolEnumType definition

ProtocolEnumType = Literal[
    "GENEVE",
    "HTTP",
    "HTTPS",
    "TCP",
    "TCP_UDP",
    "TLS",
    "UDP",
]
```
## RedirectActionStatusCodeEnumType

```python
# RedirectActionStatusCodeEnumType usage example

from types_aiobotocore_elbv2.literals import RedirectActionStatusCodeEnumType

def get_value() -> RedirectActionStatusCodeEnumType:
    return "HTTP_301"
```

```python
# RedirectActionStatusCodeEnumType definition

RedirectActionStatusCodeEnumType = Literal[
    "HTTP_301",
    "HTTP_302",
]
```
## TargetDeregisteredWaiterName

```python
# TargetDeregisteredWaiterName usage example

from types_aiobotocore_elbv2.literals import TargetDeregisteredWaiterName

def get_value() -> TargetDeregisteredWaiterName:
    return "target_deregistered"
```

```python
# TargetDeregisteredWaiterName definition

TargetDeregisteredWaiterName = Literal[
    "target_deregistered",
]
```
## TargetGroupIpAddressTypeEnumType

```python
# TargetGroupIpAddressTypeEnumType usage example

from types_aiobotocore_elbv2.literals import TargetGroupIpAddressTypeEnumType

def get_value() -> TargetGroupIpAddressTypeEnumType:
    return "ipv4"
```

```python
# TargetGroupIpAddressTypeEnumType definition

TargetGroupIpAddressTypeEnumType = Literal[
    "ipv4",
    "ipv6",
]
```
## TargetHealthReasonEnumType

```python
# TargetHealthReasonEnumType usage example

from types_aiobotocore_elbv2.literals import TargetHealthReasonEnumType

def get_value() -> TargetHealthReasonEnumType:
    return "Elb.InitialHealthChecking"
```

```python
# TargetHealthReasonEnumType definition

TargetHealthReasonEnumType = Literal[
    "Elb.InitialHealthChecking",
    "Elb.InternalError",
    "Elb.RegistrationInProgress",
    "Target.DeregistrationInProgress",
    "Target.FailedHealthChecks",
    "Target.HealthCheckDisabled",
    "Target.InvalidState",
    "Target.IpUnusable",
    "Target.NotInUse",
    "Target.NotRegistered",
    "Target.ResponseCodeMismatch",
    "Target.Timeout",
]
```
## TargetHealthStateEnumType

```python
# TargetHealthStateEnumType usage example

from types_aiobotocore_elbv2.literals import TargetHealthStateEnumType

def get_value() -> TargetHealthStateEnumType:
    return "draining"
```

```python
# TargetHealthStateEnumType definition

TargetHealthStateEnumType = Literal[
    "draining",
    "healthy",
    "initial",
    "unavailable",
    "unhealthy",
    "unused",
]
```
## TargetInServiceWaiterName

```python
# TargetInServiceWaiterName usage example

from types_aiobotocore_elbv2.literals import TargetInServiceWaiterName

def get_value() -> TargetInServiceWaiterName:
    return "target_in_service"
```

```python
# TargetInServiceWaiterName definition

TargetInServiceWaiterName = Literal[
    "target_in_service",
]
```
## TargetTypeEnumType

```python
# TargetTypeEnumType usage example

from types_aiobotocore_elbv2.literals import TargetTypeEnumType

def get_value() -> TargetTypeEnumType:
    return "alb"
```

```python
# TargetTypeEnumType definition

TargetTypeEnumType = Literal[
    "alb",
    "instance",
    "ip",
    "lambda",
]
```
## ElasticLoadBalancingv2ServiceName

```python
# ElasticLoadBalancingv2ServiceName usage example

from types_aiobotocore_elbv2.literals import ElasticLoadBalancingv2ServiceName

def get_value() -> ElasticLoadBalancingv2ServiceName:
    return "elbv2"
```

```python
# ElasticLoadBalancingv2ServiceName definition

ElasticLoadBalancingv2ServiceName = Literal[
    "elbv2",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_elbv2.literals import ServiceName

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

from types_aiobotocore_elbv2.literals import ResourceServiceName

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

from types_aiobotocore_elbv2.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_account_limits"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_account_limits",
    "describe_listener_certificates",
    "describe_listeners",
    "describe_load_balancers",
    "describe_rules",
    "describe_ssl_policies",
    "describe_target_groups",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_elbv2.literals import WaiterName

def get_value() -> WaiterName:
    return "load_balancer_available"
```

```python
# WaiterName definition

WaiterName = Literal[
    "load_balancer_available",
    "load_balancer_exists",
    "load_balancers_deleted",
    "target_deregistered",
    "target_in_service",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_elbv2.literals import RegionName

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
    "ca-central-1",
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
