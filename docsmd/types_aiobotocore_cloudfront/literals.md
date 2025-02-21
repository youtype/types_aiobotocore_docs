# Literals

> [Index](../README.md) > [CloudFront](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## CachePolicyCookieBehaviorType

```python
# CachePolicyCookieBehaviorType usage example
from types_aiobotocore_cloudfront.literals import CachePolicyCookieBehaviorType

def get_value() -> CachePolicyCookieBehaviorType:
    return "all"
```

```python
# CachePolicyCookieBehaviorType definition
CachePolicyCookieBehaviorType = Literal[
    "all",
    "allExcept",
    "none",
    "whitelist",
]
```
## CachePolicyHeaderBehaviorType

```python
# CachePolicyHeaderBehaviorType usage example
from types_aiobotocore_cloudfront.literals import CachePolicyHeaderBehaviorType

def get_value() -> CachePolicyHeaderBehaviorType:
    return "none"
```

```python
# CachePolicyHeaderBehaviorType definition
CachePolicyHeaderBehaviorType = Literal[
    "none",
    "whitelist",
]
```
## CachePolicyQueryStringBehaviorType

```python
# CachePolicyQueryStringBehaviorType usage example
from types_aiobotocore_cloudfront.literals import CachePolicyQueryStringBehaviorType

def get_value() -> CachePolicyQueryStringBehaviorType:
    return "all"
```

```python
# CachePolicyQueryStringBehaviorType definition
CachePolicyQueryStringBehaviorType = Literal[
    "all",
    "allExcept",
    "none",
    "whitelist",
]
```
## CachePolicyTypeType

```python
# CachePolicyTypeType usage example
from types_aiobotocore_cloudfront.literals import CachePolicyTypeType

def get_value() -> CachePolicyTypeType:
    return "custom"
```

```python
# CachePolicyTypeType definition
CachePolicyTypeType = Literal[
    "custom",
    "managed",
]
```
## CertificateSourceType

```python
# CertificateSourceType usage example
from types_aiobotocore_cloudfront.literals import CertificateSourceType

def get_value() -> CertificateSourceType:
    return "acm"
```

```python
# CertificateSourceType definition
CertificateSourceType = Literal[
    "acm",
    "cloudfront",
    "iam",
]
```
## ContinuousDeploymentPolicyTypeType

```python
# ContinuousDeploymentPolicyTypeType usage example
from types_aiobotocore_cloudfront.literals import ContinuousDeploymentPolicyTypeType

def get_value() -> ContinuousDeploymentPolicyTypeType:
    return "SingleHeader"
```

```python
# ContinuousDeploymentPolicyTypeType definition
ContinuousDeploymentPolicyTypeType = Literal[
    "SingleHeader",
    "SingleWeight",
]
```
## DistributionDeployedWaiterName

```python
# DistributionDeployedWaiterName usage example
from types_aiobotocore_cloudfront.literals import DistributionDeployedWaiterName

def get_value() -> DistributionDeployedWaiterName:
    return "distribution_deployed"
```

```python
# DistributionDeployedWaiterName definition
DistributionDeployedWaiterName = Literal[
    "distribution_deployed",
]
```
## EventTypeType

```python
# EventTypeType usage example
from types_aiobotocore_cloudfront.literals import EventTypeType

def get_value() -> EventTypeType:
    return "origin-request"
```

```python
# EventTypeType definition
EventTypeType = Literal[
    "origin-request",
    "origin-response",
    "viewer-request",
    "viewer-response",
]
```
## FormatType

```python
# FormatType usage example
from types_aiobotocore_cloudfront.literals import FormatType

def get_value() -> FormatType:
    return "URLEncoded"
```

```python
# FormatType definition
FormatType = Literal[
    "URLEncoded",
]
```
## FrameOptionsListType

```python
# FrameOptionsListType usage example
from types_aiobotocore_cloudfront.literals import FrameOptionsListType

def get_value() -> FrameOptionsListType:
    return "DENY"
```

```python
# FrameOptionsListType definition
FrameOptionsListType = Literal[
    "DENY",
    "SAMEORIGIN",
]
```
## FunctionRuntimeType

```python
# FunctionRuntimeType usage example
from types_aiobotocore_cloudfront.literals import FunctionRuntimeType

def get_value() -> FunctionRuntimeType:
    return "cloudfront-js-1.0"
```

```python
# FunctionRuntimeType definition
FunctionRuntimeType = Literal[
    "cloudfront-js-1.0",
    "cloudfront-js-2.0",
]
```
## FunctionStageType

```python
# FunctionStageType usage example
from types_aiobotocore_cloudfront.literals import FunctionStageType

def get_value() -> FunctionStageType:
    return "DEVELOPMENT"
```

```python
# FunctionStageType definition
FunctionStageType = Literal[
    "DEVELOPMENT",
    "LIVE",
]
```
## GeoRestrictionTypeType

```python
# GeoRestrictionTypeType usage example
from types_aiobotocore_cloudfront.literals import GeoRestrictionTypeType

def get_value() -> GeoRestrictionTypeType:
    return "blacklist"
```

```python
# GeoRestrictionTypeType definition
GeoRestrictionTypeType = Literal[
    "blacklist",
    "none",
    "whitelist",
]
```
## HttpVersionType

```python
# HttpVersionType usage example
from types_aiobotocore_cloudfront.literals import HttpVersionType

def get_value() -> HttpVersionType:
    return "http1.1"
```

```python
# HttpVersionType definition
HttpVersionType = Literal[
    "http1.1",
    "http2",
    "http2and3",
    "http3",
]
```
## ICPRecordalStatusType

```python
# ICPRecordalStatusType usage example
from types_aiobotocore_cloudfront.literals import ICPRecordalStatusType

def get_value() -> ICPRecordalStatusType:
    return "APPROVED"
```

```python
# ICPRecordalStatusType definition
ICPRecordalStatusType = Literal[
    "APPROVED",
    "PENDING",
    "SUSPENDED",
]
```
## ImportSourceTypeType

```python
# ImportSourceTypeType usage example
from types_aiobotocore_cloudfront.literals import ImportSourceTypeType

def get_value() -> ImportSourceTypeType:
    return "S3"
```

```python
# ImportSourceTypeType definition
ImportSourceTypeType = Literal[
    "S3",
]
```
## InvalidationCompletedWaiterName

```python
# InvalidationCompletedWaiterName usage example
from types_aiobotocore_cloudfront.literals import InvalidationCompletedWaiterName

def get_value() -> InvalidationCompletedWaiterName:
    return "invalidation_completed"
```

```python
# InvalidationCompletedWaiterName definition
InvalidationCompletedWaiterName = Literal[
    "invalidation_completed",
]
```
## ItemSelectionType

```python
# ItemSelectionType usage example
from types_aiobotocore_cloudfront.literals import ItemSelectionType

def get_value() -> ItemSelectionType:
    return "all"
```

```python
# ItemSelectionType definition
ItemSelectionType = Literal[
    "all",
    "none",
    "whitelist",
]
```
## ListCloudFrontOriginAccessIdentitiesPaginatorName

```python
# ListCloudFrontOriginAccessIdentitiesPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListCloudFrontOriginAccessIdentitiesPaginatorName

def get_value() -> ListCloudFrontOriginAccessIdentitiesPaginatorName:
    return "list_cloud_front_origin_access_identities"
```

```python
# ListCloudFrontOriginAccessIdentitiesPaginatorName definition
ListCloudFrontOriginAccessIdentitiesPaginatorName = Literal[
    "list_cloud_front_origin_access_identities",
]
```
## ListDistributionsPaginatorName

```python
# ListDistributionsPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListDistributionsPaginatorName

def get_value() -> ListDistributionsPaginatorName:
    return "list_distributions"
```

```python
# ListDistributionsPaginatorName definition
ListDistributionsPaginatorName = Literal[
    "list_distributions",
]
```
## ListInvalidationsPaginatorName

```python
# ListInvalidationsPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListInvalidationsPaginatorName

def get_value() -> ListInvalidationsPaginatorName:
    return "list_invalidations"
```

```python
# ListInvalidationsPaginatorName definition
ListInvalidationsPaginatorName = Literal[
    "list_invalidations",
]
```
## ListKeyValueStoresPaginatorName

```python
# ListKeyValueStoresPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListKeyValueStoresPaginatorName

def get_value() -> ListKeyValueStoresPaginatorName:
    return "list_key_value_stores"
```

```python
# ListKeyValueStoresPaginatorName definition
ListKeyValueStoresPaginatorName = Literal[
    "list_key_value_stores",
]
```
## ListPublicKeysPaginatorName

```python
# ListPublicKeysPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListPublicKeysPaginatorName

def get_value() -> ListPublicKeysPaginatorName:
    return "list_public_keys"
```

```python
# ListPublicKeysPaginatorName definition
ListPublicKeysPaginatorName = Literal[
    "list_public_keys",
]
```
## ListStreamingDistributionsPaginatorName

```python
# ListStreamingDistributionsPaginatorName usage example
from types_aiobotocore_cloudfront.literals import ListStreamingDistributionsPaginatorName

def get_value() -> ListStreamingDistributionsPaginatorName:
    return "list_streaming_distributions"
```

```python
# ListStreamingDistributionsPaginatorName definition
ListStreamingDistributionsPaginatorName = Literal[
    "list_streaming_distributions",
]
```
## MethodType

```python
# MethodType usage example
from types_aiobotocore_cloudfront.literals import MethodType

def get_value() -> MethodType:
    return "DELETE"
```

```python
# MethodType definition
MethodType = Literal[
    "DELETE",
    "GET",
    "HEAD",
    "OPTIONS",
    "PATCH",
    "POST",
    "PUT",
]
```
## MinimumProtocolVersionType

```python
# MinimumProtocolVersionType usage example
from types_aiobotocore_cloudfront.literals import MinimumProtocolVersionType

def get_value() -> MinimumProtocolVersionType:
    return "SSLv3"
```

```python
# MinimumProtocolVersionType definition
MinimumProtocolVersionType = Literal[
    "SSLv3",
    "TLSv1",
    "TLSv1.1_2016",
    "TLSv1.2_2018",
    "TLSv1.2_2019",
    "TLSv1.2_2021",
    "TLSv1_2016",
]
```
## OriginAccessControlOriginTypesType

```python
# OriginAccessControlOriginTypesType usage example
from types_aiobotocore_cloudfront.literals import OriginAccessControlOriginTypesType

def get_value() -> OriginAccessControlOriginTypesType:
    return "lambda"
```

```python
# OriginAccessControlOriginTypesType definition
OriginAccessControlOriginTypesType = Literal[
    "lambda",
    "mediapackagev2",
    "mediastore",
    "s3",
]
```
## OriginAccessControlSigningBehaviorsType

```python
# OriginAccessControlSigningBehaviorsType usage example
from types_aiobotocore_cloudfront.literals import OriginAccessControlSigningBehaviorsType

def get_value() -> OriginAccessControlSigningBehaviorsType:
    return "always"
```

```python
# OriginAccessControlSigningBehaviorsType definition
OriginAccessControlSigningBehaviorsType = Literal[
    "always",
    "never",
    "no-override",
]
```
## OriginAccessControlSigningProtocolsType

```python
# OriginAccessControlSigningProtocolsType usage example
from types_aiobotocore_cloudfront.literals import OriginAccessControlSigningProtocolsType

def get_value() -> OriginAccessControlSigningProtocolsType:
    return "sigv4"
```

```python
# OriginAccessControlSigningProtocolsType definition
OriginAccessControlSigningProtocolsType = Literal[
    "sigv4",
]
```
## OriginGroupSelectionCriteriaType

```python
# OriginGroupSelectionCriteriaType usage example
from types_aiobotocore_cloudfront.literals import OriginGroupSelectionCriteriaType

def get_value() -> OriginGroupSelectionCriteriaType:
    return "default"
```

```python
# OriginGroupSelectionCriteriaType definition
OriginGroupSelectionCriteriaType = Literal[
    "default",
    "media-quality-based",
]
```
## OriginProtocolPolicyType

```python
# OriginProtocolPolicyType usage example
from types_aiobotocore_cloudfront.literals import OriginProtocolPolicyType

def get_value() -> OriginProtocolPolicyType:
    return "http-only"
```

```python
# OriginProtocolPolicyType definition
OriginProtocolPolicyType = Literal[
    "http-only",
    "https-only",
    "match-viewer",
]
```
## OriginRequestPolicyCookieBehaviorType

```python
# OriginRequestPolicyCookieBehaviorType usage example
from types_aiobotocore_cloudfront.literals import OriginRequestPolicyCookieBehaviorType

def get_value() -> OriginRequestPolicyCookieBehaviorType:
    return "all"
```

```python
# OriginRequestPolicyCookieBehaviorType definition
OriginRequestPolicyCookieBehaviorType = Literal[
    "all",
    "allExcept",
    "none",
    "whitelist",
]
```
## OriginRequestPolicyHeaderBehaviorType

```python
# OriginRequestPolicyHeaderBehaviorType usage example
from types_aiobotocore_cloudfront.literals import OriginRequestPolicyHeaderBehaviorType

def get_value() -> OriginRequestPolicyHeaderBehaviorType:
    return "allExcept"
```

```python
# OriginRequestPolicyHeaderBehaviorType definition
OriginRequestPolicyHeaderBehaviorType = Literal[
    "allExcept",
    "allViewer",
    "allViewerAndWhitelistCloudFront",
    "none",
    "whitelist",
]
```
## OriginRequestPolicyQueryStringBehaviorType

```python
# OriginRequestPolicyQueryStringBehaviorType usage example
from types_aiobotocore_cloudfront.literals import OriginRequestPolicyQueryStringBehaviorType

def get_value() -> OriginRequestPolicyQueryStringBehaviorType:
    return "all"
```

```python
# OriginRequestPolicyQueryStringBehaviorType definition
OriginRequestPolicyQueryStringBehaviorType = Literal[
    "all",
    "allExcept",
    "none",
    "whitelist",
]
```
## OriginRequestPolicyTypeType

```python
# OriginRequestPolicyTypeType usage example
from types_aiobotocore_cloudfront.literals import OriginRequestPolicyTypeType

def get_value() -> OriginRequestPolicyTypeType:
    return "custom"
```

```python
# OriginRequestPolicyTypeType definition
OriginRequestPolicyTypeType = Literal[
    "custom",
    "managed",
]
```
## PriceClassType

```python
# PriceClassType usage example
from types_aiobotocore_cloudfront.literals import PriceClassType

def get_value() -> PriceClassType:
    return "PriceClass_100"
```

```python
# PriceClassType definition
PriceClassType = Literal[
    "PriceClass_100",
    "PriceClass_200",
    "PriceClass_All",
]
```
## RealtimeMetricsSubscriptionStatusType

```python
# RealtimeMetricsSubscriptionStatusType usage example
from types_aiobotocore_cloudfront.literals import RealtimeMetricsSubscriptionStatusType

def get_value() -> RealtimeMetricsSubscriptionStatusType:
    return "Disabled"
```

```python
# RealtimeMetricsSubscriptionStatusType definition
RealtimeMetricsSubscriptionStatusType = Literal[
    "Disabled",
    "Enabled",
]
```
## ReferrerPolicyListType

```python
# ReferrerPolicyListType usage example
from types_aiobotocore_cloudfront.literals import ReferrerPolicyListType

def get_value() -> ReferrerPolicyListType:
    return "no-referrer"
```

```python
# ReferrerPolicyListType definition
ReferrerPolicyListType = Literal[
    "no-referrer",
    "no-referrer-when-downgrade",
    "origin",
    "origin-when-cross-origin",
    "same-origin",
    "strict-origin",
    "strict-origin-when-cross-origin",
    "unsafe-url",
]
```
## ResponseHeadersPolicyAccessControlAllowMethodsValuesType

```python
# ResponseHeadersPolicyAccessControlAllowMethodsValuesType usage example
from types_aiobotocore_cloudfront.literals import ResponseHeadersPolicyAccessControlAllowMethodsValuesType

def get_value() -> ResponseHeadersPolicyAccessControlAllowMethodsValuesType:
    return "ALL"
```

```python
# ResponseHeadersPolicyAccessControlAllowMethodsValuesType definition
ResponseHeadersPolicyAccessControlAllowMethodsValuesType = Literal[
    "ALL",
    "DELETE",
    "GET",
    "HEAD",
    "OPTIONS",
    "PATCH",
    "POST",
    "PUT",
]
```
## ResponseHeadersPolicyTypeType

```python
# ResponseHeadersPolicyTypeType usage example
from types_aiobotocore_cloudfront.literals import ResponseHeadersPolicyTypeType

def get_value() -> ResponseHeadersPolicyTypeType:
    return "custom"
```

```python
# ResponseHeadersPolicyTypeType definition
ResponseHeadersPolicyTypeType = Literal[
    "custom",
    "managed",
]
```
## SSLSupportMethodType

```python
# SSLSupportMethodType usage example
from types_aiobotocore_cloudfront.literals import SSLSupportMethodType

def get_value() -> SSLSupportMethodType:
    return "sni-only"
```

```python
# SSLSupportMethodType definition
SSLSupportMethodType = Literal[
    "sni-only",
    "static-ip",
    "vip",
]
```
## SslProtocolType

```python
# SslProtocolType usage example
from types_aiobotocore_cloudfront.literals import SslProtocolType

def get_value() -> SslProtocolType:
    return "SSLv3"
```

```python
# SslProtocolType definition
SslProtocolType = Literal[
    "SSLv3",
    "TLSv1",
    "TLSv1.1",
    "TLSv1.2",
]
```
## StreamingDistributionDeployedWaiterName

```python
# StreamingDistributionDeployedWaiterName usage example
from types_aiobotocore_cloudfront.literals import StreamingDistributionDeployedWaiterName

def get_value() -> StreamingDistributionDeployedWaiterName:
    return "streaming_distribution_deployed"
```

```python
# StreamingDistributionDeployedWaiterName definition
StreamingDistributionDeployedWaiterName = Literal[
    "streaming_distribution_deployed",
]
```
## ViewerProtocolPolicyType

```python
# ViewerProtocolPolicyType usage example
from types_aiobotocore_cloudfront.literals import ViewerProtocolPolicyType

def get_value() -> ViewerProtocolPolicyType:
    return "allow-all"
```

```python
# ViewerProtocolPolicyType definition
ViewerProtocolPolicyType = Literal[
    "allow-all",
    "https-only",
    "redirect-to-https",
]
```
## CloudFrontServiceName

```python
# CloudFrontServiceName usage example
from types_aiobotocore_cloudfront.literals import CloudFrontServiceName

def get_value() -> CloudFrontServiceName:
    return "cloudfront"
```

```python
# CloudFrontServiceName definition
CloudFrontServiceName = Literal[
    "cloudfront",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_cloudfront.literals import ServiceName

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
from types_aiobotocore_cloudfront.literals import ResourceServiceName

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
from types_aiobotocore_cloudfront.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_cloud_front_origin_access_identities"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_cloud_front_origin_access_identities",
    "list_distributions",
    "list_invalidations",
    "list_key_value_stores",
    "list_public_keys",
    "list_streaming_distributions",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_cloudfront.literals import WaiterName

def get_value() -> WaiterName:
    return "distribution_deployed"
```

```python
# WaiterName definition
WaiterName = Literal[
    "distribution_deployed",
    "invalidation_completed",
    "streaming_distribution_deployed",
]
```
