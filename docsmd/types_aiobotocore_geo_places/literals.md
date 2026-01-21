# Literals

> [Index](../README.md) > [LocationServicePlacesV2](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2)
    type annotations stubs module [types-aiobotocore-geo-places](https://pypi.org/project/types-aiobotocore-geo-places/).

## AutocompleteAdditionalFeatureType

```python
# AutocompleteAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import AutocompleteAdditionalFeatureType

def get_value() -> AutocompleteAdditionalFeatureType:
    return "Core"
```

```python
# AutocompleteAdditionalFeatureType definition
AutocompleteAdditionalFeatureType = Literal[
    "Core",
]
```
## AutocompleteFilterPlaceTypeType

```python
# AutocompleteFilterPlaceTypeType usage example
from types_aiobotocore_geo_places.literals import AutocompleteFilterPlaceTypeType

def get_value() -> AutocompleteFilterPlaceTypeType:
    return "Locality"
```

```python
# AutocompleteFilterPlaceTypeType definition
AutocompleteFilterPlaceTypeType = Literal[
    "Locality",
    "PostalCode",
]
```
## AutocompleteIntendedUseType

```python
# AutocompleteIntendedUseType usage example
from types_aiobotocore_geo_places.literals import AutocompleteIntendedUseType

def get_value() -> AutocompleteIntendedUseType:
    return "SingleUse"
```

```python
# AutocompleteIntendedUseType definition
AutocompleteIntendedUseType = Literal[
    "SingleUse",
]
```
## GeocodeAdditionalFeatureType

```python
# GeocodeAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import GeocodeAdditionalFeatureType

def get_value() -> GeocodeAdditionalFeatureType:
    return "Access"
```

```python
# GeocodeAdditionalFeatureType definition
GeocodeAdditionalFeatureType = Literal[
    "Access",
    "Intersections",
    "SecondaryAddresses",
    "TimeZone",
]
```
## GeocodeFilterPlaceTypeType

```python
# GeocodeFilterPlaceTypeType usage example
from types_aiobotocore_geo_places.literals import GeocodeFilterPlaceTypeType

def get_value() -> GeocodeFilterPlaceTypeType:
    return "InterpolatedAddress"
```

```python
# GeocodeFilterPlaceTypeType definition
GeocodeFilterPlaceTypeType = Literal[
    "InterpolatedAddress",
    "Intersection",
    "Locality",
    "PointAddress",
    "PostalCode",
    "Street",
]
```
## GeocodeIntendedUseType

```python
# GeocodeIntendedUseType usage example
from types_aiobotocore_geo_places.literals import GeocodeIntendedUseType

def get_value() -> GeocodeIntendedUseType:
    return "SingleUse"
```

```python
# GeocodeIntendedUseType definition
GeocodeIntendedUseType = Literal[
    "SingleUse",
    "Storage",
]
```
## GetPlaceAdditionalFeatureType

```python
# GetPlaceAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import GetPlaceAdditionalFeatureType

def get_value() -> GetPlaceAdditionalFeatureType:
    return "Access"
```

```python
# GetPlaceAdditionalFeatureType definition
GetPlaceAdditionalFeatureType = Literal[
    "Access",
    "Contact",
    "Phonemes",
    "SecondaryAddresses",
    "TimeZone",
]
```
## GetPlaceIntendedUseType

```python
# GetPlaceIntendedUseType usage example
from types_aiobotocore_geo_places.literals import GetPlaceIntendedUseType

def get_value() -> GetPlaceIntendedUseType:
    return "SingleUse"
```

```python
# GetPlaceIntendedUseType definition
GetPlaceIntendedUseType = Literal[
    "SingleUse",
    "Storage",
]
```
## PlaceTypeType

```python
# PlaceTypeType usage example
from types_aiobotocore_geo_places.literals import PlaceTypeType

def get_value() -> PlaceTypeType:
    return "Block"
```

```python
# PlaceTypeType definition
PlaceTypeType = Literal[
    "Block",
    "Country",
    "District",
    "InferredSecondaryAddress",
    "InterpolatedAddress",
    "Intersection",
    "Locality",
    "PointAddress",
    "PointOfInterest",
    "PostalCode",
    "Region",
    "SecondaryAddress",
    "Street",
    "SubBlock",
    "SubDistrict",
    "SubRegion",
]
```
## PostalAuthorityType

```python
# PostalAuthorityType usage example
from types_aiobotocore_geo_places.literals import PostalAuthorityType

def get_value() -> PostalAuthorityType:
    return "Usps"
```

```python
# PostalAuthorityType definition
PostalAuthorityType = Literal[
    "Usps",
]
```
## PostalCodeModeType

```python
# PostalCodeModeType usage example
from types_aiobotocore_geo_places.literals import PostalCodeModeType

def get_value() -> PostalCodeModeType:
    return "EnumerateSpannedLocalities"
```

```python
# PostalCodeModeType definition
PostalCodeModeType = Literal[
    "EnumerateSpannedLocalities",
    "MergeAllSpannedLocalities",
]
```
## PostalCodeTypeType

```python
# PostalCodeTypeType usage example
from types_aiobotocore_geo_places.literals import PostalCodeTypeType

def get_value() -> PostalCodeTypeType:
    return "UspsZip"
```

```python
# PostalCodeTypeType definition
PostalCodeTypeType = Literal[
    "UspsZip",
    "UspsZipPlus4",
]
```
## QueryTypeType

```python
# QueryTypeType usage example
from types_aiobotocore_geo_places.literals import QueryTypeType

def get_value() -> QueryTypeType:
    return "BusinessChain"
```

```python
# QueryTypeType definition
QueryTypeType = Literal[
    "BusinessChain",
    "Category",
]
```
## RecordTypeCodeType

```python
# RecordTypeCodeType usage example
from types_aiobotocore_geo_places.literals import RecordTypeCodeType

def get_value() -> RecordTypeCodeType:
    return "Firm"
```

```python
# RecordTypeCodeType definition
RecordTypeCodeType = Literal[
    "Firm",
    "General",
    "HighRise",
    "PostOfficeBox",
    "Rural",
    "Street",
]
```
## ReverseGeocodeAdditionalFeatureType

```python
# ReverseGeocodeAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import ReverseGeocodeAdditionalFeatureType

def get_value() -> ReverseGeocodeAdditionalFeatureType:
    return "Access"
```

```python
# ReverseGeocodeAdditionalFeatureType definition
ReverseGeocodeAdditionalFeatureType = Literal[
    "Access",
    "Intersections",
    "TimeZone",
]
```
## ReverseGeocodeFilterPlaceTypeType

```python
# ReverseGeocodeFilterPlaceTypeType usage example
from types_aiobotocore_geo_places.literals import ReverseGeocodeFilterPlaceTypeType

def get_value() -> ReverseGeocodeFilterPlaceTypeType:
    return "InterpolatedAddress"
```

```python
# ReverseGeocodeFilterPlaceTypeType definition
ReverseGeocodeFilterPlaceTypeType = Literal[
    "InterpolatedAddress",
    "Intersection",
    "Locality",
    "PointAddress",
    "Street",
]
```
## ReverseGeocodeIntendedUseType

```python
# ReverseGeocodeIntendedUseType usage example
from types_aiobotocore_geo_places.literals import ReverseGeocodeIntendedUseType

def get_value() -> ReverseGeocodeIntendedUseType:
    return "SingleUse"
```

```python
# ReverseGeocodeIntendedUseType definition
ReverseGeocodeIntendedUseType = Literal[
    "SingleUse",
    "Storage",
]
```
## SearchNearbyAdditionalFeatureType

```python
# SearchNearbyAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import SearchNearbyAdditionalFeatureType

def get_value() -> SearchNearbyAdditionalFeatureType:
    return "Access"
```

```python
# SearchNearbyAdditionalFeatureType definition
SearchNearbyAdditionalFeatureType = Literal[
    "Access",
    "Contact",
    "Phonemes",
    "TimeZone",
]
```
## SearchNearbyIntendedUseType

```python
# SearchNearbyIntendedUseType usage example
from types_aiobotocore_geo_places.literals import SearchNearbyIntendedUseType

def get_value() -> SearchNearbyIntendedUseType:
    return "SingleUse"
```

```python
# SearchNearbyIntendedUseType definition
SearchNearbyIntendedUseType = Literal[
    "SingleUse",
    "Storage",
]
```
## SearchTextAdditionalFeatureType

```python
# SearchTextAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import SearchTextAdditionalFeatureType

def get_value() -> SearchTextAdditionalFeatureType:
    return "Access"
```

```python
# SearchTextAdditionalFeatureType definition
SearchTextAdditionalFeatureType = Literal[
    "Access",
    "Contact",
    "Phonemes",
    "TimeZone",
]
```
## SearchTextIntendedUseType

```python
# SearchTextIntendedUseType usage example
from types_aiobotocore_geo_places.literals import SearchTextIntendedUseType

def get_value() -> SearchTextIntendedUseType:
    return "SingleUse"
```

```python
# SearchTextIntendedUseType definition
SearchTextIntendedUseType = Literal[
    "SingleUse",
    "Storage",
]
```
## SuggestAdditionalFeatureType

```python
# SuggestAdditionalFeatureType usage example
from types_aiobotocore_geo_places.literals import SuggestAdditionalFeatureType

def get_value() -> SuggestAdditionalFeatureType:
    return "Access"
```

```python
# SuggestAdditionalFeatureType definition
SuggestAdditionalFeatureType = Literal[
    "Access",
    "Core",
    "Phonemes",
    "TimeZone",
]
```
## SuggestIntendedUseType

```python
# SuggestIntendedUseType usage example
from types_aiobotocore_geo_places.literals import SuggestIntendedUseType

def get_value() -> SuggestIntendedUseType:
    return "SingleUse"
```

```python
# SuggestIntendedUseType definition
SuggestIntendedUseType = Literal[
    "SingleUse",
]
```
## SuggestResultItemTypeType

```python
# SuggestResultItemTypeType usage example
from types_aiobotocore_geo_places.literals import SuggestResultItemTypeType

def get_value() -> SuggestResultItemTypeType:
    return "Place"
```

```python
# SuggestResultItemTypeType definition
SuggestResultItemTypeType = Literal[
    "Place",
    "Query",
]
```
## TypePlacementType

```python
# TypePlacementType usage example
from types_aiobotocore_geo_places.literals import TypePlacementType

def get_value() -> TypePlacementType:
    return "AfterBaseName"
```

```python
# TypePlacementType definition
TypePlacementType = Literal[
    "AfterBaseName",
    "BeforeBaseName",
]
```
## ZipClassificationCodeType

```python
# ZipClassificationCodeType usage example
from types_aiobotocore_geo_places.literals import ZipClassificationCodeType

def get_value() -> ZipClassificationCodeType:
    return "Military"
```

```python
# ZipClassificationCodeType definition
ZipClassificationCodeType = Literal[
    "Military",
    "PostOfficeBoxes",
    "Unique",
]
```
## LocationServicePlacesV2ServiceName

```python
# LocationServicePlacesV2ServiceName usage example
from types_aiobotocore_geo_places.literals import LocationServicePlacesV2ServiceName

def get_value() -> LocationServicePlacesV2ServiceName:
    return "geo-places"
```

```python
# LocationServicePlacesV2ServiceName definition
LocationServicePlacesV2ServiceName = Literal[
    "geo-places",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_geo_places.literals import ServiceName

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
from types_aiobotocore_geo_places.literals import ResourceServiceName

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
