# Literals

> [Index](../README.md) > [AlexaForBusiness](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AlexaForBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
    type annotations stubs module [types-aiobotocore-alexaforbusiness](https://pypi.org/project/types-aiobotocore-alexaforbusiness/).

## BusinessReportFailureCodeType

```python
# BusinessReportFailureCodeType usage example

from types_aiobotocore_alexaforbusiness.literals import BusinessReportFailureCodeType

def get_value() -> BusinessReportFailureCodeType:
    return "ACCESS_DENIED"
```

```python
# BusinessReportFailureCodeType definition

BusinessReportFailureCodeType = Literal[
    "ACCESS_DENIED",
    "INTERNAL_FAILURE",
    "NO_SUCH_BUCKET",
]
```
## BusinessReportFormatType

```python
# BusinessReportFormatType usage example

from types_aiobotocore_alexaforbusiness.literals import BusinessReportFormatType

def get_value() -> BusinessReportFormatType:
    return "CSV"
```

```python
# BusinessReportFormatType definition

BusinessReportFormatType = Literal[
    "CSV",
    "CSV_ZIP",
]
```
## BusinessReportIntervalType

```python
# BusinessReportIntervalType usage example

from types_aiobotocore_alexaforbusiness.literals import BusinessReportIntervalType

def get_value() -> BusinessReportIntervalType:
    return "ONE_DAY"
```

```python
# BusinessReportIntervalType definition

BusinessReportIntervalType = Literal[
    "ONE_DAY",
    "ONE_WEEK",
    "THIRTY_DAYS",
]
```
## BusinessReportStatusType

```python
# BusinessReportStatusType usage example

from types_aiobotocore_alexaforbusiness.literals import BusinessReportStatusType

def get_value() -> BusinessReportStatusType:
    return "FAILED"
```

```python
# BusinessReportStatusType definition

BusinessReportStatusType = Literal[
    "FAILED",
    "RUNNING",
    "SUCCEEDED",
]
```
## CommsProtocolType

```python
# CommsProtocolType usage example

from types_aiobotocore_alexaforbusiness.literals import CommsProtocolType

def get_value() -> CommsProtocolType:
    return "H323"
```

```python
# CommsProtocolType definition

CommsProtocolType = Literal[
    "H323",
    "SIP",
    "SIPS",
]
```
## ConferenceProviderTypeType

```python
# ConferenceProviderTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import ConferenceProviderTypeType

def get_value() -> ConferenceProviderTypeType:
    return "BLUEJEANS"
```

```python
# ConferenceProviderTypeType definition

ConferenceProviderTypeType = Literal[
    "BLUEJEANS",
    "CHIME",
    "CUSTOM",
    "FUZE",
    "GOOGLE_HANGOUTS",
    "POLYCOM",
    "RINGCENTRAL",
    "SKYPE_FOR_BUSINESS",
    "WEBEX",
    "ZOOM",
]
```
## ConnectionStatusType

```python
# ConnectionStatusType usage example

from types_aiobotocore_alexaforbusiness.literals import ConnectionStatusType

def get_value() -> ConnectionStatusType:
    return "OFFLINE"
```

```python
# ConnectionStatusType definition

ConnectionStatusType = Literal[
    "OFFLINE",
    "ONLINE",
]
```
## DeviceEventTypeType

```python
# DeviceEventTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import DeviceEventTypeType

def get_value() -> DeviceEventTypeType:
    return "CONNECTION_STATUS"
```

```python
# DeviceEventTypeType definition

DeviceEventTypeType = Literal[
    "CONNECTION_STATUS",
    "DEVICE_STATUS",
]
```
## DeviceStatusDetailCodeType

```python
# DeviceStatusDetailCodeType usage example

from types_aiobotocore_alexaforbusiness.literals import DeviceStatusDetailCodeType

def get_value() -> DeviceStatusDetailCodeType:
    return "ASSOCIATION_REJECTION"
```

```python
# DeviceStatusDetailCodeType definition

DeviceStatusDetailCodeType = Literal[
    "ASSOCIATION_REJECTION",
    "AUTHENTICATION_FAILURE",
    "CERTIFICATE_AUTHORITY_ACCESS_DENIED",
    "CERTIFICATE_ISSUING_LIMIT_EXCEEDED",
    "CREDENTIALS_ACCESS_FAILURE",
    "DEVICE_SOFTWARE_UPDATE_NEEDED",
    "DEVICE_WAS_OFFLINE",
    "DHCP_FAILURE",
    "DNS_FAILURE",
    "INTERNET_UNAVAILABLE",
    "INVALID_CERTIFICATE_AUTHORITY",
    "INVALID_PASSWORD_STATE",
    "NETWORK_PROFILE_NOT_FOUND",
    "PASSWORD_MANAGER_ACCESS_DENIED",
    "PASSWORD_NOT_FOUND",
    "TLS_VERSION_MISMATCH",
    "UNKNOWN_FAILURE",
]
```
## DeviceStatusType

```python
# DeviceStatusType usage example

from types_aiobotocore_alexaforbusiness.literals import DeviceStatusType

def get_value() -> DeviceStatusType:
    return "DEREGISTERED"
```

```python
# DeviceStatusType definition

DeviceStatusType = Literal[
    "DEREGISTERED",
    "FAILED",
    "PENDING",
    "READY",
    "WAS_OFFLINE",
]
```
## DeviceUsageTypeType

```python
# DeviceUsageTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import DeviceUsageTypeType

def get_value() -> DeviceUsageTypeType:
    return "VOICE"
```

```python
# DeviceUsageTypeType definition

DeviceUsageTypeType = Literal[
    "VOICE",
]
```
## DistanceUnitType

```python
# DistanceUnitType usage example

from types_aiobotocore_alexaforbusiness.literals import DistanceUnitType

def get_value() -> DistanceUnitType:
    return "IMPERIAL"
```

```python
# DistanceUnitType definition

DistanceUnitType = Literal[
    "IMPERIAL",
    "METRIC",
]
```
## EnablementTypeFilterType

```python
# EnablementTypeFilterType usage example

from types_aiobotocore_alexaforbusiness.literals import EnablementTypeFilterType

def get_value() -> EnablementTypeFilterType:
    return "ENABLED"
```

```python
# EnablementTypeFilterType definition

EnablementTypeFilterType = Literal[
    "ENABLED",
    "PENDING",
]
```
## EnablementTypeType

```python
# EnablementTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import EnablementTypeType

def get_value() -> EnablementTypeType:
    return "ENABLED"
```

```python
# EnablementTypeType definition

EnablementTypeType = Literal[
    "ENABLED",
    "PENDING",
]
```
## EndOfMeetingReminderTypeType

```python
# EndOfMeetingReminderTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import EndOfMeetingReminderTypeType

def get_value() -> EndOfMeetingReminderTypeType:
    return "ANNOUNCEMENT_TIME_CHECK"
```

```python
# EndOfMeetingReminderTypeType definition

EndOfMeetingReminderTypeType = Literal[
    "ANNOUNCEMENT_TIME_CHECK",
    "ANNOUNCEMENT_VARIABLE_TIME_LEFT",
    "CHIME",
    "KNOCK",
]
```
## EnrollmentStatusType

```python
# EnrollmentStatusType usage example

from types_aiobotocore_alexaforbusiness.literals import EnrollmentStatusType

def get_value() -> EnrollmentStatusType:
    return "DEREGISTERING"
```

```python
# EnrollmentStatusType definition

EnrollmentStatusType = Literal[
    "DEREGISTERING",
    "DISASSOCIATING",
    "INITIALIZED",
    "PENDING",
    "REGISTERED",
]
```
## FeatureType

```python
# FeatureType usage example

from types_aiobotocore_alexaforbusiness.literals import FeatureType

def get_value() -> FeatureType:
    return "ALL"
```

```python
# FeatureType definition

FeatureType = Literal[
    "ALL",
    "BLUETOOTH",
    "LISTS",
    "NETWORK_PROFILE",
    "NOTIFICATIONS",
    "SETTINGS",
    "SKILLS",
    "VOLUME",
]
```
## ListBusinessReportSchedulesPaginatorName

```python
# ListBusinessReportSchedulesPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListBusinessReportSchedulesPaginatorName

def get_value() -> ListBusinessReportSchedulesPaginatorName:
    return "list_business_report_schedules"
```

```python
# ListBusinessReportSchedulesPaginatorName definition

ListBusinessReportSchedulesPaginatorName = Literal[
    "list_business_report_schedules",
]
```
## ListConferenceProvidersPaginatorName

```python
# ListConferenceProvidersPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListConferenceProvidersPaginatorName

def get_value() -> ListConferenceProvidersPaginatorName:
    return "list_conference_providers"
```

```python
# ListConferenceProvidersPaginatorName definition

ListConferenceProvidersPaginatorName = Literal[
    "list_conference_providers",
]
```
## ListDeviceEventsPaginatorName

```python
# ListDeviceEventsPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListDeviceEventsPaginatorName

def get_value() -> ListDeviceEventsPaginatorName:
    return "list_device_events"
```

```python
# ListDeviceEventsPaginatorName definition

ListDeviceEventsPaginatorName = Literal[
    "list_device_events",
]
```
## ListSkillsPaginatorName

```python
# ListSkillsPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListSkillsPaginatorName

def get_value() -> ListSkillsPaginatorName:
    return "list_skills"
```

```python
# ListSkillsPaginatorName definition

ListSkillsPaginatorName = Literal[
    "list_skills",
]
```
## ListSkillsStoreCategoriesPaginatorName

```python
# ListSkillsStoreCategoriesPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListSkillsStoreCategoriesPaginatorName

def get_value() -> ListSkillsStoreCategoriesPaginatorName:
    return "list_skills_store_categories"
```

```python
# ListSkillsStoreCategoriesPaginatorName definition

ListSkillsStoreCategoriesPaginatorName = Literal[
    "list_skills_store_categories",
]
```
## ListSkillsStoreSkillsByCategoryPaginatorName

```python
# ListSkillsStoreSkillsByCategoryPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListSkillsStoreSkillsByCategoryPaginatorName

def get_value() -> ListSkillsStoreSkillsByCategoryPaginatorName:
    return "list_skills_store_skills_by_category"
```

```python
# ListSkillsStoreSkillsByCategoryPaginatorName definition

ListSkillsStoreSkillsByCategoryPaginatorName = Literal[
    "list_skills_store_skills_by_category",
]
```
## ListSmartHomeAppliancesPaginatorName

```python
# ListSmartHomeAppliancesPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListSmartHomeAppliancesPaginatorName

def get_value() -> ListSmartHomeAppliancesPaginatorName:
    return "list_smart_home_appliances"
```

```python
# ListSmartHomeAppliancesPaginatorName definition

ListSmartHomeAppliancesPaginatorName = Literal[
    "list_smart_home_appliances",
]
```
## ListTagsPaginatorName

```python
# ListTagsPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import ListTagsPaginatorName

def get_value() -> ListTagsPaginatorName:
    return "list_tags"
```

```python
# ListTagsPaginatorName definition

ListTagsPaginatorName = Literal[
    "list_tags",
]
```
## LocaleType

```python
# LocaleType usage example

from types_aiobotocore_alexaforbusiness.literals import LocaleType

def get_value() -> LocaleType:
    return "en-US"
```

```python
# LocaleType definition

LocaleType = Literal[
    "en-US",
]
```
## NetworkEapMethodType

```python
# NetworkEapMethodType usage example

from types_aiobotocore_alexaforbusiness.literals import NetworkEapMethodType

def get_value() -> NetworkEapMethodType:
    return "EAP_TLS"
```

```python
# NetworkEapMethodType definition

NetworkEapMethodType = Literal[
    "EAP_TLS",
]
```
## NetworkSecurityTypeType

```python
# NetworkSecurityTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import NetworkSecurityTypeType

def get_value() -> NetworkSecurityTypeType:
    return "OPEN"
```

```python
# NetworkSecurityTypeType definition

NetworkSecurityTypeType = Literal[
    "OPEN",
    "WEP",
    "WPA2_ENTERPRISE",
    "WPA2_PSK",
    "WPA_PSK",
]
```
## PhoneNumberTypeType

```python
# PhoneNumberTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import PhoneNumberTypeType

def get_value() -> PhoneNumberTypeType:
    return "HOME"
```

```python
# PhoneNumberTypeType definition

PhoneNumberTypeType = Literal[
    "HOME",
    "MOBILE",
    "WORK",
]
```
## RequirePinType

```python
# RequirePinType usage example

from types_aiobotocore_alexaforbusiness.literals import RequirePinType

def get_value() -> RequirePinType:
    return "NO"
```

```python
# RequirePinType definition

RequirePinType = Literal[
    "NO",
    "OPTIONAL",
    "YES",
]
```
## SearchDevicesPaginatorName

```python
# SearchDevicesPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import SearchDevicesPaginatorName

def get_value() -> SearchDevicesPaginatorName:
    return "search_devices"
```

```python
# SearchDevicesPaginatorName definition

SearchDevicesPaginatorName = Literal[
    "search_devices",
]
```
## SearchProfilesPaginatorName

```python
# SearchProfilesPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import SearchProfilesPaginatorName

def get_value() -> SearchProfilesPaginatorName:
    return "search_profiles"
```

```python
# SearchProfilesPaginatorName definition

SearchProfilesPaginatorName = Literal[
    "search_profiles",
]
```
## SearchRoomsPaginatorName

```python
# SearchRoomsPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import SearchRoomsPaginatorName

def get_value() -> SearchRoomsPaginatorName:
    return "search_rooms"
```

```python
# SearchRoomsPaginatorName definition

SearchRoomsPaginatorName = Literal[
    "search_rooms",
]
```
## SearchSkillGroupsPaginatorName

```python
# SearchSkillGroupsPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import SearchSkillGroupsPaginatorName

def get_value() -> SearchSkillGroupsPaginatorName:
    return "search_skill_groups"
```

```python
# SearchSkillGroupsPaginatorName definition

SearchSkillGroupsPaginatorName = Literal[
    "search_skill_groups",
]
```
## SearchUsersPaginatorName

```python
# SearchUsersPaginatorName usage example

from types_aiobotocore_alexaforbusiness.literals import SearchUsersPaginatorName

def get_value() -> SearchUsersPaginatorName:
    return "search_users"
```

```python
# SearchUsersPaginatorName definition

SearchUsersPaginatorName = Literal[
    "search_users",
]
```
## SipTypeType

```python
# SipTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import SipTypeType

def get_value() -> SipTypeType:
    return "WORK"
```

```python
# SipTypeType definition

SipTypeType = Literal[
    "WORK",
]
```
## SkillTypeFilterType

```python
# SkillTypeFilterType usage example

from types_aiobotocore_alexaforbusiness.literals import SkillTypeFilterType

def get_value() -> SkillTypeFilterType:
    return "ALL"
```

```python
# SkillTypeFilterType definition

SkillTypeFilterType = Literal[
    "ALL",
    "PRIVATE",
    "PUBLIC",
]
```
## SkillTypeType

```python
# SkillTypeType usage example

from types_aiobotocore_alexaforbusiness.literals import SkillTypeType

def get_value() -> SkillTypeType:
    return "PRIVATE"
```

```python
# SkillTypeType definition

SkillTypeType = Literal[
    "PRIVATE",
    "PUBLIC",
]
```
## SortValueType

```python
# SortValueType usage example

from types_aiobotocore_alexaforbusiness.literals import SortValueType

def get_value() -> SortValueType:
    return "ASC"
```

```python
# SortValueType definition

SortValueType = Literal[
    "ASC",
    "DESC",
]
```
## TemperatureUnitType

```python
# TemperatureUnitType usage example

from types_aiobotocore_alexaforbusiness.literals import TemperatureUnitType

def get_value() -> TemperatureUnitType:
    return "CELSIUS"
```

```python
# TemperatureUnitType definition

TemperatureUnitType = Literal[
    "CELSIUS",
    "FAHRENHEIT",
]
```
## WakeWordType

```python
# WakeWordType usage example

from types_aiobotocore_alexaforbusiness.literals import WakeWordType

def get_value() -> WakeWordType:
    return "ALEXA"
```

```python
# WakeWordType definition

WakeWordType = Literal[
    "ALEXA",
    "AMAZON",
    "COMPUTER",
    "ECHO",
]
```
## AlexaForBusinessServiceName

```python
# AlexaForBusinessServiceName usage example

from types_aiobotocore_alexaforbusiness.literals import AlexaForBusinessServiceName

def get_value() -> AlexaForBusinessServiceName:
    return "alexaforbusiness"
```

```python
# AlexaForBusinessServiceName definition

AlexaForBusinessServiceName = Literal[
    "alexaforbusiness",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_alexaforbusiness.literals import ServiceName

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

from types_aiobotocore_alexaforbusiness.literals import ResourceServiceName

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

from types_aiobotocore_alexaforbusiness.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_business_report_schedules"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_business_report_schedules",
    "list_conference_providers",
    "list_device_events",
    "list_skills",
    "list_skills_store_categories",
    "list_skills_store_skills_by_category",
    "list_smart_home_appliances",
    "list_tags",
    "search_devices",
    "search_profiles",
    "search_rooms",
    "search_skill_groups",
    "search_users",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_alexaforbusiness.literals import RegionName

def get_value() -> RegionName:
    return "us-east-1"
```

```python
# RegionName definition

RegionName = Literal[
    "us-east-1",
]
```
